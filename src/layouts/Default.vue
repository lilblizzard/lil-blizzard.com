<template>
  <div class="layout">
    <header class="header">
      <strong>
        <g-link class="home__link" to="/">{{ $static.metadata.siteName }}</g-link>
      </strong>
      <g-image class="nav__logo" to="/" src="~/images/snowflake-45.svg" width="200" />
      <nav class="nav">
        <g-link class="nav__link" to="/">Home</g-link>
        <g-link class="nav__link" to="/code/">Code</g-link>
        <g-link class="nav__link" to="/music/">Music</g-link>
        <g-link class="nav__link" to="/contact/">Contact</g-link>
      </nav>
    </header>
    <slot />
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style>
body {
  font-family: -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Roboto,
    "Helvetica Neue", Arial, sans-serif;
  margin: 0;
  padding: 0;
  line-height: 1.5;
}

.layout {
  max-width: 50rem;
  margin: 0 auto;
  padding-left: 1rem;
  padding-right: 1rem;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 1rem;
  height: 5rem;
}

.nav__link {
  margin-left: 1rem;
  text-decoration: none;
  color: black;
}

.nav__link.active--exact.active {
  text-decoration: underline;
}

.home__link {
  color: black;
  padding-right: 0.4rem;
}

.nav__logo {
  margin-right: auto;
  animation: rotation 30s infinite linear;
  transform-origin: center;
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
