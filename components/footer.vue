<template>
  <section>
    <b-container class="bv-example-row">
      <b-row>
        <b-col class="text-white">
          <h2>Contact</h2>
          <p style="color: #5c7ae4">Make an appointment</p>
          <p>
            <b-col cols="0.5">
              <a class="social-phone" href="www.google.com"> 06 12 34 56 78</a> <br /> <br>
              <a class="social-whatsapp" href="www.whatsapp.com"> 06 12 34 56 78</a> <br /> <br>
              <a class="social-insta" href="www.instagram.com"> @develokey</a> <br /> <br>
            </b-col>
          </p>
        </b-col>
        <b-col class="text-white">
          <form class="mobile mb-3" action="/action_page.php">
            <label class="text-white" for="fname">First name:</label><br />
            <input
              class="text-white"
              type="text"
              id="fname"
              name="fname"
            /><br />
            <label class="text-white" for="lname">Last name:</label><br />
            <input
              class="text-white"
              type="text"
              id="lname"
              name="lname"
            /><br /><br />
            <label class="text-white" for="lname">Subject:</label><br />
            <input
              class="text-white"
              type="text"
              id="subject"
              name="subject"
            /><br /><br />
            <label class="text-white" for="lname">Message:</label><br />
            <input
              class="text-white"
              type="text"
              id="msg"
              name="msg"
            /><br /><br />
            <input
              class="text-white btn btn-outline-primary"
              type="submit"
              value="Send mail"
            />
          </form>
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<style lang="css" scoped>
section {
  margin-bottom: 3rem;
}

input {
  width: 600px;
  background-color: transparent;
  border: none;
  border-bottom: 1px solid #5c7ae4;
}

input::active {
  border: none !important;
}

.social-phone::before {
  content: url("././assets/img/svg/phone.svg");
  cursor: pointer;
}

.social-whatsapp::before {
  content: url("././assets/img/svg/whatsapp.svg");
  cursor: pointer;
}

.social-insta::before {
  content: url("././assets/img/svg/insta.svg");
  cursor: pointer;
}

@media only screen and (max-width: 767px) and (min-width: 300px) {
  .mobile input {
    width: 90%
  }
}


</style>