<template>
  <section>
    <div class="hero">
      <div>
        <h1 class="text-white text-center">Lorem Ipsum</h1>

        <p class="text-white text-center">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae fuga
          <br />
          voluptatibus accusantium eos quisquam aliquam ducimus error sit omnis,
          <br />
          dignissimos cum officiis quibusdam aspernatur dolores temporibus quod
          <br />
          explicabo praesentium cupiditate!
        </p>
        <div class="d-flex justify-content-center"></div>
      </div>
    </div>
    <div class="container">
      <div
        :style="{
          backgroundColor: checkASelected ? 'green' : 'transparent',
          background: crossASelected ? 'red' : 'transparent',
        }"
        class="item border-white text-white"
      >
        <i @click="checkSelected('A')" class="fas fa-check fa-3x"></i>
        <div>ITEM</div>
        <div>
          <i @click="crossSelected('A')" class="fas fa-times fa-3x"></i>
        </div>
      </div>
      <div
        :style="{
          backgroundColor: checkBSelected ? 'green' : 'transparent',
          background: crossBSelected ? 'red' : 'transparent',
        }"
        class="item border-white text-white"
      >
        <i @click="checkSelected('B')" class="fas fa-check fa-3x"></i>

        <div>ITEM</div>
        <div>
          <i @click="crossSelected('B')" class="fas fa-times fa-3x"></i>
        </div>
      </div>
      <div
        :style="{
          backgroundColor: checkCSelected ? 'green' : 'transparent',
          background: crossCSelected ? 'red' : 'transparent',
        }"
        class="item border-white text-white"
      >
        <i @click="checkSelected('C')" class="fas fa-check fa-3x"></i>

        <div>ITEM</div>
        <div>
          <i @click="crossSelected('C')" class="fas fa-times fa-3x"></i>
        </div>
      </div>
      <div
        :style="{
          backgroundColor: checkDSelected ? 'green' : 'transparent',
          background: crossDSelected ? 'red' : 'transparent',
        }"
        class="item border-white text-white"
      >
        <i @click="checkSelected('D')" class="fas fa-check fa-3x"></i>

        <div>ITEM</div>
        <div>
          <i @click="crossSelected('D')" class="fas fa-times fa-3x"></i>
        </div>
      </div>
      <div
        :style="{
          backgroundColor: checkESelected ? 'green' : 'transparent',
          background: crossESelected ? 'red' : 'transparent',
        }"
        class="item border-white text-white"
      >
        <i @click="checkSelected('E')" class="fas fa-check fa-3x"></i>

        <div>ITEM</div>
        <div>
          <i @click="crossSelected('E')" class="fas fa-times fa-3x"></i>
        </div>
      </div>

      <div
        :style="{
          backgroundColor: checkFSelected ? 'green' : 'transparent',
          background: crossFSelected ? 'red' : 'transparent',
        }"
        class="item border-white text-white"
      >
        <i @click="checkSelected('F')" class="fas fa-check fa-3x"></i>

        <div>ITEM</div>
        <div>
          <i @click="crossSelected('F')" class="fas fa-times fa-3x"></i>
        </div>
      </div>

      <div
        :style="{
          backgroundColor: checkGSelected ? 'green' : 'transparent',
          background: crossGSelected ? 'red' : 'transparent',
        }"
        class="item border-white text-white"
      >
        <i @click="checkSelected('G')" class="fas fa-check fa-3x"></i>

        <div>ITEM</div>
        <div>
          <i @click="crossSelected('G')" class="fas fa-times fa-3x"></i>
        </div>
      </div>
      <div
        :style="{
          backgroundColor: checkHSelected ? 'green' : 'transparent',
          background: crossHSelected ? 'red' : 'transparent',
        }"
        class="item border-white text-white"
      >
        <i @click="checkSelected('H')" class="fas fa-check fa-3x"></i>

        <div>ITEM H</div>
        <div>
          <i @click="crossSelected('H')" class="fas fa-times fa-3x"></i>
        </div>
      </div>
    </div>
  </section>
</template>
<style lang="css" scoped>
.item {
  width: 100%;
  display: flex;
  justify-content: space-between;
  border: 1px solid white;
  border-radius: 3px;
  padding: 3%;
}

.container {
  display: flex;
  flex-wrap: wrap;
}

.container > div {
  flex: 50%; /* or - flex: 0 50% - or - flex-basis: 50% - */
  /*demo*/
  box-shadow: 0 0 0 1px black;
  margin-bottom: 10px;
}

.cross {
  background-color: red;
}

.check {
  background-color: green;
}
</style>
// backgroundColor: crossASelected ? 'red' : 'transparent'

<script>
export default {
  data() {
    return {
      checkASelected: false,
      checkBSelected: false,
      checkCSelected: false,
      checkDSelected: false,
      checkESelected: false,
      checkFSelected: false,
      checkGSelected: false,
      checkHSelected: false,
      // here ends the checks and starts the crosses
      crossASelected: false,
      crossBSelected: false,
      crossCSelected: false,
      crossDSelected: false,
      crossESelected: false,
      crossFSelected: false,
      crossGSelected: false,
      crossHSelected: false,
    };
  },
  methods: {
    checkSelected(check) {
      console.log(check)
      if (check === "A") {
        this.checkASelected = true
      } else if (check === "B") {
        this.checkBSelected = true
      } else if (check === "C") {
        this.checkBSelected = true
      } else if (check === "D") {
        this.checkBSelected = true
      } else if (check === "E") {
        this.checkBSelected = true
      } else if (check === "F") {
        this.checkBSelected = true
      } else if (check === "G") {
        this.checkBSelected = true
      } else if (check === "H") {
        this.checkBSelected = true
      }
    },

    crossSelected(cross) {
      console.log(cross)
      if (cross === "A") {
        this.crossASelected = true;
      } else if (cross === "B") {
        this.crossBSelected = true;
      } else if (cross === "C") {
        this.crossBSelected = true;
      } else if (cross === "D") {
        this.crossBSelected = true;
      } else if (cross === "E") {
        this.crossBSelected = true;
      } else if (cross === "F") {
        this.crossBSelected = true;
      } else if (cross === "G") {
        this.crossBSelected = true;
      } else if (cross === "H") {
        this.crossBSelected = true;
      }
    },

    // crossySelected(cross) {
    //   switch (cross === "A") {
    //     case cross === "A":
    //       this.crossASelected = true;
    //       break;
    //     case cross === "B":
    //       this.crossBSelected = true;
    //       break;
    //     case cross === "C":
    //       this.crossCSelected = true;
    //       break;
    //     case cross === "D":
    //       this.crossDSelected = true;
    //       break;
    //     case cross === "E":
    //       this.crossESelected = true;
    //       break;
    //     case cross === "F":
    //       this.crossFSelected = true;
    //       break;
    //     case cross === "G":
    //       this.crossGSelected = true;
    //       break;
    //     case cross === "H":
    //       this.crossHSelected = true;
    //       break;
    //     default:
    //       break;
    //   }
    // },
  },
};
</script>
