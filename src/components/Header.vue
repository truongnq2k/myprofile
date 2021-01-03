<template>
  <div class="header">
    <nav class="navbar navbar-expand-lg navbar-light bg-light shadow">
      <div class="container">
        <router-link class="navbar-brand" to="/">
          <font-awesome-icon class="text-success" icon="code" size="1x" /> TDEVS
        </router-link>

        <button
          class="navbar-toggler collapsed"
          type="button"
          data-toggle="collapse"
          data-target="#navbarSupportedContent"
        >
          <div class="hamburger-toggle">
            <div class="hamburger">
              <span></span>
              <span></span>
              <span></span>
            </div>
          </div>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav mr-auto mb-2 mb-lg-0">
            <li class="nav-item"></li>
            <li class="nav-item">
              <router-link class="nav-link" to="/about">About</router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
@charset "UTF-8";
@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

.navbar-toggler {
  border: none;
  padding: 0;
  outline: none;
}
.navbar-toggler:focus {
  box-shadow: none;
}
.navbar-toggler .hamburger-toggle {
  position: relative;
  display: inline-block;
  width: 50px;
  height: 50px;
  z-index: 11;
  float: right;
}
.navbar-toggler .hamburger-toggle .hamburger {
  position: absolute;
  transform: translate(-50%, -50%) rotate(0deg);
  left: 50%;
  top: 50%;
  width: 50%;
  height: 50%;
  pointer-events: none;
}
.navbar-toggler .hamburger-toggle .hamburger span {
  width: 100%;
  height: 4px;
  position: absolute;
  background: #333;
  border-radius: 2px;
  z-index: 1;
  transition: transform 0.2s cubic-bezier(0.77, 0.2, 0.05, 1),
    background 0.2s cubic-bezier(0.77, 0.2, 0.05, 1), all 0.2s ease-in-out;
  left: 0px;
}
.navbar-toggler .hamburger-toggle .hamburger span:first-child {
  top: 10%;
  transform-origin: 50% 50%;
  transform: translate(0% -50%) !important;
}
.navbar-toggler .hamburger-toggle .hamburger span:nth-child(2) {
  top: 50%;
  transform: translate(0, -50%);
}
.navbar-toggler .hamburger-toggle .hamburger span:last-child {
  left: 0px;
  top: auto;
  bottom: 10%;
  transform-origin: 50% 50%;
}
.navbar-toggler .hamburger-toggle .hamburger.active span {
  position: absolute;
  margin: 0;
}
.navbar-toggler .hamburger-toggle .hamburger.active span:first-child {
  top: 45%;
  transform: rotate(45deg);
}
.navbar-toggler .hamburger-toggle .hamburger.active span:nth-child(2) {
  left: 50%;
  width: 0px;
}
.navbar-toggler .hamburger-toggle .hamburger.active span:last-child {
  top: 45%;
  transform: rotate(-45deg);
}
</style>