<template>
  <section>
    <link rel="stylesheet" href=".././assets/styles/styles.css" />
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css"
    />
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
        text-variant="light"
        bg-variant="dark"
        :backdrop-variant="variant"
        backdrop
        shadow
      >
        <a class="card  text-white bg-dark" href="/">
          <div class="px-3 py-2"><i class="fas fa-home"></i> Home</div></a
        >
        <a class="card  text-white bg-dark mt-3" href="/About">
          <div class="px-3 py-2">
            <i class="fas fa-info-circle"></i> About
          </div></a
        >
        <a class="card  text-white bg-dark mt-3" href="/services">
          <div class="px-3 py-2">
            <i class="fas fa-keyboard"></i> Services
          </div></a
        >
        <a class="card  text-white bg-dark mt-3" href="/contact">
          <div class="px-3 py-2">
            <i class="fas fa-address-card"></i> Contact
          </div></a
        >
        <a class="card  text-white bg-dark mt-3" href="/gym">
          <div class="px-3 py-2">
            <i class="fas fa-dumbbell"></i> gym
          </div></a
        >
      </b-sidebar>
    </div>
    <hr class="solid i-know-you-are-looking" />
  </section>
</template>

<script>
export default {
  data() {
    return {
      variant: "primary",
    };
  },
};
</script>

<style lang="css" scoped>
section {
  margin-bottom: 2rem;
}

hr.solid {
  border-top: 1px solid #e1e45c;
  opacity: 50%;
}
</style>

