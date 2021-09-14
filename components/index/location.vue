<template>
  <section>
    <b-container class="bv-example-row">
      <b-row>
        <b-col class="text-white">
          <iframe
            id="map"
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d15447.102861560237!2d4.483204015207343!3d52.16057733997295!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47c642489521527b%3A0x9f4852fc4854709!2sBurcht%20van%20Leiden!5e0!3m2!1snl!2snl!4v1631516351306!5m2!1snl!2snl"
            width="600"
            height="300"
            style="border: 0;  filter: grayscale(50%) invert(92%) contrast(83%);"
            allowfullscreen=""
            loading="lazy"
            alt="google maps"
          ></iframe>
        </b-col>
        <b-col class="text-white mobile">
          <h2>
            Lorem ipsum
            <span
              ><script src="https://cdn.lordicon.com/libs/mssddfmo/lord-icon-2.1.0.js"></script>
              <lord-icon
                src="https://cdn.lordicon.com/zzcjjxew.json"
                trigger="hover"
                colors="primary:#eee966,secondary:#eee966"
                style="width: 45px; height: 45px"
              >
              </lord-icon
            ></span>
          </h2>
          <p>
            spanLorem ipsum dolor sit amet consectetur adipisicing elit. Maxime
            unde quidem neque magni distinctio veniam ab, perferendis quasi
            harum quisquam aperiam itaque commodi sunt qui non modi repellendus.
            Recusandae, odio.nihil magni voluptatem totam nihil magni voluptatem
            totam     

          </p>
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<style lang="css" scoped>
section {
  margin-bottom: 5rem;
  margin-top: 5rem;
}
@media only screen and (max-width: 767px) and (min-width: 300px) {
  .mobile {
    display: none;
  }
}
iframe {
  border-radius: 5px;
}
</style>

<script>
// do not delete this is usefull for later

// export default {
//   data() { 
//     return {
//       names: ['John', 'Carlos', 'Matt'] 
//     }
//   },
//   computed: {
//     randomName() {
//       let n = this.names.length
//       let randomNumber = Math.floor(Math.random() * n)
//       return this.names[randomNumber]
//     }
//   }
// }
</script>
