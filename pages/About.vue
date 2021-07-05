<template>
  <div>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/vue/1.0.18/vue.min.js"></script>

    <nav class="navbar navbar-dark bg-success">
      <button
        v-b-toggle.sidebar-backdrop
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#navbarToggleExternalContent"
        aria-controls="navbarToggleExternalContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
    </nav>
    <b-sidebar
      id="sidebar-backdrop"
      title="Menu"
      :backdrop-variant="variant"
      backdrop
      shadow
    >
      <a class="card" href="/"> <div class="px-3 py-2">Home</div></a>
      <a class="card mt-3" href=""> <div class="px-3 py-2">About</div></a>
      <a class="card mt-3" href=""> <div class="px-3 py-2">hello</div></a>
      <a class="card mt-3" href=""> <div class="px-3 py-2">hello</div></a>
    </b-sidebar>
  </div>
</template>

