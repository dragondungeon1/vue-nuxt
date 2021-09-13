<template>
  <section>
    <b-container class="bv-example-row">
      <b-row>
        <b-col cols="0.5">
          <a class="social-phone" href="www.google.com"></a> <br />
          <a class="social-whatsapp" href="www.whatsapp.com"></a> <br />
          <a class="social-insta" href="www.instagram.com"></a> <br />
        </b-col>
        <b-col class="text-white">
          <h2>Lorem ipsum</h2>
          <p style="color:#E1E45C">Lorem ipsum</p>

          <p>
            spanLorem ipsum dolor sit amet consectetur adipisicing elit. Maxime
            unde quidem neque magni distinctio veniam ab, perferendis quasi
            harum quisquam aperiam itaque commodi sunt qui non modi repellendus.
            Recusandae, odio.nihil magni voluptatem totam nihil magni voluptatem
            totam
          </p>
          <a class="btn btn-outline-primary" href="#">Learn more</a>
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
    <br /><br /><br /><br /><br />
  </section>
</template>

<script>
export default {};
</script>

<style lang="css" scoped>
.big {
  max-width: 80%;
}

p {
  font-weight: 100;
}
.social-phone::before {
  content: url("../../assets/img/svg/phone.svg");
  cursor: pointer;
}

.social-whatsapp::before {
  content: url("../../assets/img/svg/whatsapp.svg");
  cursor: pointer;
}

.social-insta::before {
  content: url("../../assets/img/svg/insta.svg");
  cursor: pointer;
}

section {
  margin-bottom: 2rem;
}

@media only screen and (max-width: 767px) and (min-width: 300px)  {
    .mobile{
        display: none;
    }
}
</style>
