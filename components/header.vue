<template>
  <div>
    <div>
      <!-- <button class="nav-collapse btn btn-primary">click me</button> -->
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
       <a class="card mt-3" href="/About"> <div class="px-3 py-2">About</div></a>
       <a class="card mt-3" href=""> <div class="px-3 py-2">hello</div></a>
       <a class="card mt-3" href=""> <div class="px-3 py-2">hello</div></a>
      </b-sidebar>
    </div>
    <div>
      <b-container class="bv-example-row mb-3 mt-5">
        <b-row align-h="around">
          <b-col cols="6">
            <div>
              <h2>Lorem ipsum</h2>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
                enim ad minim veniam, quis nostrud exercitation ullamco laboris
                nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor
                in reprehenderit in voluptate velit esse cillum dolore eu fugiat
                nulla pariatur.
              </p>
            </div>
          </b-col>
          <b-col cols="6">One of two columns</b-col>
        </b-row>
      </b-container>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      variant: "success"
    };
  }
};
</script>

<style scoped>
.card:hover {
  border: 1px solid lightgreen;
  transition: ease-in 0.2s;
}
a {
  text-decoration: none;
  color: green;
}

</style>
