<template>
<section>
   <link rel="stylesheet" href=".././assets/styles/styles.css">
    <div>
      <nav class="navbar navbar-dark">
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
        <h4 class="text-white">Lorem ipsum</h4>

      </nav>

      <b-sidebar
        id="sidebar-backdrop"
        title="Menu"
        :backdrop-variant="variant"
        backdrop
        shadow
      >
       <a class="card" href="/"> <div class="px-3 py-2">Home</div></a>
       <a class="card mt-3" href="/About"> <div class="px-3 py-2">About</div></a>
       <a class="card mt-3" href=""> <div class="px-3 py-2">hello</div></a>
       <a class="card mt-3" href=""> <div class="px-3 py-2">hello</div></a>
      </b-sidebar>
    </div>
    <hr class="solid" />

  </section> 
</template>

<script>
export default {
  data() {
    return {
      variant: "primary"
    };
  }
};
</script>

<style lang="css" scoped>
section{
  margin-bottom: 2rem;
}

hr.solid {
  border-top: 1px solid #E1E45C;
  opacity: 50%;
}
</style>

