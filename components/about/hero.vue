<template>
  <section>
    <b-container class="bv-example-row">
      <b-row>
        <b-col class="text-white">
          <h2>About ipsum</h2>
          <p style="color: #e1e45c">Lorem ipsum</p>

          <p>
            spanLorem ipsum dolor sit amet consectetur adipisicing elit. Maxime
            unde quidem neque magni distinctio veniam ab, perferendis quasi
            harum quisquam aperiam itaque commodi sunt qui non modi repellendus.
            Recusandae, odio.nihil magni voluptatem totam nihil magni voluptatem
            totam
          </p>
          <div>
            <a class="btn btn-outline-primary" href="#">
            <lord-icon
              src="https://cdn.lordicon.com/dxjqoygy.json"
              trigger="hover"
              colors="primary:#ffff,secondary:#ffff"
              style="width: 40px; height: 40px"
              target="div"
            >
            </lord-icon>
            make an appointment
            <script src="https://cdn.lordicon.com/libs/mssddfmo/lord-icon-2.1.0.js"></script>
          </a>
          </div>
          
        </b-col>
        <b-col class="text-white text-center mobile">
          <b-img
            class="big"
            src="../../assets/img/png/hero.png"
            fluid
            alt="Responsive image"
          ></b-img>
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<style lang="css" scoped>
section {
  margin-bottom: 2rem;
  margin-top: 2rem;
}

@media only screen and (max-width: 767px) and (min-width: 300px) {
  .mobile {
    display: none;
  }
}
</style>