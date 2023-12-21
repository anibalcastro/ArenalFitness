<!-- Sidebar.vue -->
<template>
  <div class="cMenu" >
    <b-button class="btnMenu" v-b-toggle.sidebar-no-header>Menú</b-button>
    <b-sidebar id="sidebar-no-header" aria-labelledby="sidebar-no-header-title" no-header shadow>
      <template #default="{ hide }">
        <div class="p-3">
          <h4 id="sidebar-no-header-title">Custom header sidebar</h4>
          <p>
            Cras mattis consectetur purus sit amet fermentum. Cras justo odio, dapibus ac facilisis
            in, egestas eget quam. Morbi leo risus, porta ac consectetur ac, vestibulum at eros.
          </p>
          <nav class="mb-3">
            <b-nav vertical>
              <b-nav-item active @click="hide">Active</b-nav-item>
              <b-nav-item href="#link-1" @click="hide">Link</b-nav-item>
              <b-nav-item href="#link-2" @click="hide">Another Link</b-nav-item>
            </b-nav>
          </nav>
          <b-button variant="primary" block @click="hide">Close Sidebar</b-button>
        </div>
      </template>
    </b-sidebar>
  </div>
</template>

<script>
export default {
  name: "AppSidebar",
  props: {
    msg: String,
  },
};
</script>

<style>
/* Estilos específicos del componente si es necesario */
.vertical-menu {
  width: 200px;
  background-color: #f4f4f4;
  padding: 10px;
}

.vertical-menu a {
  display: block;
  padding: 8px;
  text-decoration: none;
  color: #333;
  border-bottom: 1px solid #ccc;
  display: flex;
  flex-direction: column;
}

.vertical-menu a:hover {
  background-color: #ddd;
}

.cMenu{
  margin: 0;
  height: 50px;
  width: 100%;
  background-color: #4c7dac;
  display: flex;
  align-items: center;
  justify-content: flex-start;
}

.btnMenu{
  margin-left: 10px;
  width: 100px;
  height: 40px;
  background-color: white !important;
  color: black !important;
}
</style>
