<template>
  <section>
    <div class="area" >
      <ul class="circles">
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
      </ul>
    </div >
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

.circles {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  overflow: hidden;
}

.circles li {
  position: absolute;
  display: block;
  list-style: none;
  width: 20px;
  height: 20px;
  background: rgba(255, 255, 255, 0.2);
  animation: animate 25s linear infinite;
  bottom: -150px;

}

.circles li:nth-child(1) {
  left: 25%;
  width: 80px;
  height: 80px;
  animation-delay: 0s;
}


.circles li:nth-child(2) {
  left: 10%;
  width: 20px;
  height: 20px;
  animation-delay: 2s;
  animation-duration: 12s;
}

.circles li:nth-child(3) {
  left: 70%;
  width: 20px;
  height: 20px;
  animation-delay: 4s;
}

.circles li:nth-child(4) {
  left: 40%;
  width: 60px;
  height: 60px;
  animation-delay: 0s;
  animation-duration: 18s;
}

.circles li:nth-child(5) {
  left: 65%;
  width: 20px;
  height: 20px;
  animation-delay: 0s;
}

.circles li:nth-child(6) {
  left: 75%;
  width: 110px;
  height: 110px;
  animation-delay: 3s;
}

.circles li:nth-child(7) {
  left: 35%;
  width: 150px;
  height: 150px;
  animation-delay: 7s;
}

.circles li:nth-child(8) {
  left: 50%;
  width: 25px;
  height: 25px;
  animation-delay: 15s;
  animation-duration: 45s;
}

.circles li:nth-child(9) {
  left: 20%;
  width: 15px;
  height: 15px;
  animation-delay: 2s;
  animation-duration: 35s;
}

.circles li:nth-child(10) {
  left: 85%;
  width: 150px;
  height: 150px;
  animation-delay: 0s;
  animation-duration: 11s;
}

@keyframes animate {

  0% {
    transform: translateY(0) rotate(0deg);
    opacity: 1;
    border-radius: 0;
  }

  100% {
    transform: translateY(-1000px) rotate(720deg);
    opacity: 0;
    border-radius: 50%;
  }

}

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
