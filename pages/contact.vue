<template>
  <div class="container">
    <form ref="form" @submit.prevent="sendEmail">
      <label>name</label>
      <input type="text" name="user_name" />
      <label>email</label>
      <input type="email" name="user_email" />
      <label>message</label>
      <textarea name="message"></textarea>
      <input type="submit" value="Send" />
    </form>
  </div>
</template>

<script>
import emailjs from "emailjs-com";

export default {
    data() {
        return {
            email: "",
            name: "",
            message: ""
        }
    },

  methods: {
    sendEmail() {
      emailjs
        .sendForm(
          "service_ck7lv1h",
          "template_j641qge",
          this.$refs.form,
          "user_xzAl4tedcukr4FdEcS2Wb"
        )
        .then(
          (result) => {
            console.log("SUCCESS!", result.text);
          },
          (error) => {
            console.log("FAILED...", error.text);
          },
        );
    },
    resetInput() {
        this.email = "",
        this.message = "",
        this.name = ""
    }
  },
};
</script>

<style scoped lang="css">
* {
  box-sizing: border-box;
}

.container {
  display: block;
  margin: auto;
  text-align: center;
  border-radius: 5px;
  background-color: #f2f2f2;
  padding: 20px;
  width: 50%;
}

label {
  float: left;
}

input[type="text"],
[type="email"],
textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 4px;
  box-sizing: border-box;
  margin-top: 6px;
  margin-bottom: 16px;
  resize: vertical;
}

input[type="submit"] {
  background-color: #4caf50;
  color: white;
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

input[type="submit"]:hover {
  background-color: #45a049;
}
</style>
