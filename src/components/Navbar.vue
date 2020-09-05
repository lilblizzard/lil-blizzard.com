<template>
  <div>
    <header class="header">
      <g-image class="nav__logo" to="/" src="~/images/snowflake-45.svg" width="200" />
      <nav class="nav">
        <!-- maybe put image outside of nav & wrap in div -->
        <g-link class="nav__link" to="/">Home</g-link>
        <g-link class="nav__link" to="/code/">Code</g-link>
        <g-link class="nav__link" to="/music/">Music</g-link>
        <g-link class="nav__link" to="/contact/">Contact</g-link>
      </nav>
    </header>
  </div>
</template>

<script>
export default {}
</script>

<style>
.header {
  border-bottom: 1px solid rgba(83, 83, 83, 0.1);
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 5rem;
}
.nav__logo {
  margin-right: auto;
  animation: rotation 30s infinite linear;
  transform-origin: center;
}
.nav__link {
  margin-left: 1rem;
  text-decoration: none;
  color: black;
}
.nav__link.active--exact.active {
  text-decoration: underline;
}
@keyframes rotation {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(359deg);
  }
}
</style>
