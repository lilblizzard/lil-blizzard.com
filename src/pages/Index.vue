<template>
  <Layout>
    <h1 class="hero__title">Patrick Perkins</h1>
    <g-image class="hero__image" src="~/images/profile.jpg" />
    <p class="hero__text">
      a.k.a lil blizzard - composer, programmer, designer based in philly.
      currently working with old books and new tech.
    </p>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Home',
  },
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
.hero__title {
  font-size: 3rem;
  margin: 0 auto;
  margin-top: 0.5rem;
  margin-bottom: 0.5rem;
}
.hero__image {
  max-width: 100%;
  max-height: 20rem;
  object-fit: cover;
  border-radius: 0.5rem;
}
.hero__text {
  font-size: 1.1rem;
  border: 1px solid rgba(255, 255, 255, 0.2);
  border-radius: 0.5rem;
  padding: 0.5rem;
  margin: 0 auto;
  margin-top: 0.5rem;
}
</style>
