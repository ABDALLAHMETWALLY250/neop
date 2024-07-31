<template>
  <nav class="navbar px-3 fixed_top">
    <div class="container-fluid">
      <router-link class="navbar-brand" to="/">
        <img src="@/assets/images/Frame.png" alt="" />
      </router-link>
      <div class="d-flex align-items-center justify-content-center gap-2">
        <span class="cart">
          <img src="@/assets/images/cart.png" alt="" />
        </span>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="offcanvas"
          data-bs-target="#offcanvasNavbar"
          aria-controls="offcanvasNavbar"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
      </div>
      <div
        class="offcanvas offcanvas-end"
        tabindex="-1"
        id="offcanvasNavbar"
        aria-labelledby="offcanvasNavbarLabel"
      >
        <div class="offcanvas-header">
          <h5 class="offcanvas-title" id="offcanvasNavbarLabel">Offcanvas</h5>
          <button
            type="button"
            class="btn-close"
            data-bs-dismiss="offcanvas"
            aria-label="Close"
          ></button>
        </div>
        <div class="offcanvas-body">
          <ul class="navbar-nav justify-content-end flex-grow-1 pe-3">
            <li class="nav-item">
              <router-link class="nav-link" to="/" active-class="active"
                >Home</router-link
              >
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/task" active-class="active"
                >Task</router-link
              >
            </li>
          </ul>
        </div>
      </div>
    </div>
  </nav>
</template>


<style lang="scss" scoped>
button.navbar-toggler {
  border: unset;
}
.cart {
  background: #004876;
  border-radius: 50px;
  width: 32px;
  height: 32px;
  text-align: center;
  line-height: 1.8;
  color: white;
}
</style>