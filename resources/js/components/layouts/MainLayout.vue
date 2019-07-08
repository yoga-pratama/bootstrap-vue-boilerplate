<template>
  <div>
    <navbar-component></navbar-component>
    <div class="container-fluid">
      <div class="row">
        <sidebar-component></sidebar-component>
        <main role="main" class="col-md-9 ml-sm-auto col-lg-10 pt-3 px-4">
          <slot></slot>
        </main>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: "main-layout",
  mounted() {
    
  }
};
</script>

