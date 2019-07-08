<template>
  <nav class="col-md-2 d-none d-md-block bg-light sidebar">
    <div class="sidebar-sticky">
      <h6
        class="sidebar-heading d-flex justify-content-between align-items-center px-3 mt-4 mb-1 text-muted"
      >
        <span>Menu</span>
        <a class="d-flex align-items-center text-muted" href="#">
          <span class="fa fa-book-open"></span>
        </a>
      </h6>
      <ul class="nav flex-column">
        <li class="nav-item">
          <router-link class="nav-link" to="/Menu" exact>
            <span class="fa fa-archive"></span>
            Menu 1
          </router-link>
        </li>

        <li class="nav-item">
          <router-link class="nav-link" to="/MENU2" exact>
            <span class="fa fa-align-justify"></span>
            Menu 2
          </router-link>
        </li>
      </ul>

      <h6
        class="sidebar-heading d-flex justify-content-between align-items-center px-3 mt-4 mb-1 text-muted"
      >
        <span>Admin Menu</span>
        <a class="d-flex align-items-center text-muted" href="#">
          <span class="fa fa-book-open"></span>
        </a>
      </h6>
      <ul class="nav flex-column mb-2">
        <li class="nav-item">
          <router-link to="/user" class="nav-link">
            <span class="fa fa-user"></span>
            User
          </router-link>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: "sidebar"
};
</script>
