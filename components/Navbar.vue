<template>
  <nav>
    <div class="nav-container">
      <span class="logo">
        <NuxtLink to="/">Movie Info</NuxtLink>
      </span>
      <ul class="menu-items">
        <li class="menu-item">
          <NuxtLink to="/">Home</NuxtLink>
        </li>
        <li class="menu-item">
          <NuxtLink to="/movies">Movies</NuxtLink>
        </li>
        <li class="menu-item">
          <NuxtLink to="/tv-shows">TV Shows</NuxtLink>
        </li>
        <li class="menu-item">
          <NuxtLink to="/popular-people">People</NuxtLink>
        </li>
      </ul>
    </div>
  </nav>
</template>

<style scoped>
@import "~/assets/design/custom/components/navbar.css";
</style>
