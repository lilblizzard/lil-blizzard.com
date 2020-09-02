<template>
  <Layout>
    <h1>Patrick Perkins</h1>
    <g-image class="hero" src="~/images/profile.jpg" />
    <p>a.k.a lil-blizzard. composer, programmer, designer based in philly. currently working with old books and new tech.</p>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: "Home",
  },
};
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
.hero {
  max-width: 100%;
  max-height: 20rem;
  object-fit: cover;
}
</style>
