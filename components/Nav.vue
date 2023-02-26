<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <NuxtLink class="navbar-brand" to="/">Firengii</NuxtLink>
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarSupportedContent"
      aria-controls="navbarSupportedContent"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse ml-auto" id="navbarSupportedContent">
      <ul class="navbar-nav ml-auto">
        <li class="nav-item active">
          <Nuxt-link href="/products" to="/products" class="nav-link"
            >Products<span class="sr-only">(current)</span></Nuxt-link
          >
        </li>
        <li class="nav-item active">
          <Nuxt-link to="/my-items" class="nav-link"
            >My items<span class="sr-only">(current)</span></Nuxt-link
          >
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {};
</script>

<style></style>
