<template>
  <div class="container-fluid p-0 position-fixed" >
    <header
      class="d-flex flex-wrap align-items-center justify-content-center px-2 justify-content-md-between m-0"
      style="background-color: #333!important;
    box-shadow: rgba(0,0,0,.25) 0 3px 11px 0!important;
    -moz-box-shadow: rgba(0,0,0,.25) 0 3px 11px 0!important;
    -webkit-box-shadow: rgba(0,0,0,.25) 0 3px 11px 0!important;"
    >
      <a
        href="/"
        class="d-flex align-items-center col-md-3 mb-2 mb-md-0 text-dark text-decoration-none"
      >
        <img src="../../assets/tgsf_color_5-490w.png" style="width: 200px" />
      </a>

      <ul class="navbar-nav d-flex flex-row">
        <li><a href="#" class="nav-link px-2 link-secondary">Home</a></li>
        <li class="nav-item dropdown">
          <a
            class="nav-link px-2 link-light dropdown-toggle"
            href="#"
            id="navbarDarkDropdownMenuLink"
            role="button"
            data-bs-toggle="dropdown"
            aria-expanded="false"
          >
            Meetings & Events
          </a>
          <ul
            class="dropdown-menu dropdown-menu-dark"
            aria-labelledby="navbarDarkDropdownMenuLink"
          >
            <li><a class="dropdown-item" href="#">Photo Gallery</a></li>
          </ul>
        </li>
        <li class="nav-item dropdown">
          <a
            class="nav-link px-2 link-light dropdown-toggle"
            href="#"
            id="navbarDarkDropdownMenuLink"
            role="button"
            data-bs-toggle="dropdown"
            aria-expanded="false"
          >
            About Us
          </a>
          <ul
            class="dropdown-menu dropdown-menu-dark"
            aria-labelledby="navbarDarkDropdownMenuLink"
          >
            <li><a class="dropdown-item" href="#">Charter Members</a></li>
          </ul>
        </li>
        <li><a href="#" class="nav-link px-2 link-light">Current News</a></li>
        <li><a href="#" class="nav-link px-2 link-light">Contact Us</a></li>
        <li><a href="#" class="nav-link px-2 link-light">Forms</a></li>
      </ul>
    </header>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style lang="scss" scoped>
</style>