<template>
  <section>
    <div class="container">
      <div :style="{backgroundColor: checkASelected ? 'green' : 'transparent', backgroundColor: crossASelected ? 'red' : 'transparent'}"   class="item border-white text-white">
        <i @click="checkSelected('A')" class="fas fa-check fa-3x"></i>

        <div>ITEM</div>
        <div><i @click="crossSelected('A')" class=" fas fa-times fa-3x"></i></div>
      </div>
      <div class="item border-white text-white">
        <i class=" fas fa-check fa-3x"></i>

        <div>ITEM</div>
        <div><i class=" fas fa-times fa-3x"></i></div>
      </div>
      <div class="item border-white text-white">
        <i class=" fas fa-check fa-3x"></i>

        <div>ITEM</div>
        <div><i class=" fas fa-times fa-3x"></i></div>
      </div>
      <div class="item border-white text-white">
        <i class=" fas fa-check fa-3x"></i>

        <div>ITEM</div>
        <div><i class=" fas fa-times fa-3x"></i></div>
      </div>
      <div class="item border-white text-white">
        <i class=" fas fa-check fa-3x"></i>

        <div>ITEM</div>
        <div><i class=" fas fa-times fa-3x"></i></div>
      </div>

      <div class="item border-white text-white">
        <i class=" fas fa-check fa-3x"></i>

        <div>ITEM</div>
        <div><i class=" fas fa-times fa-3x"></i></div>
      </div>

      <div class="item border-white text-white">
        <i class=" fas fa-check fa-3x"></i>

        <div>ITEM</div>
        <div><i class=" fas fa-times fa-3x"></i></div>
      </div>
      <div class="item border-white text-white">
        <i class=" fas fa-check fa-3x"></i>

        <div>ITEM</div>
        <div><i class=" fas fa-times fa-3x"></i></div>
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

.check{
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
            if (check === 'A') {
                this.checkASelected = true
            }else if (check === 'B') {
                this.checkBSelected = true
            }else if (check === 'C') {
                this.checkBSelected = true
            }else if (check === 'D') {
                this.checkBSelected = true
            }else if (check === 'E') {
                this.checkBSelected = true
            }else if (check === 'F') {
                this.checkBSelected = true
            }else if (check === 'G') {
                this.checkBSelected = true
            }else if (check === 'H') {
                this.checkBSelected = true
            }
        },

        crossSelected(cross) {
            if (cross === 'A') {
                this.crossASelected = true
            }else if (cross === 'B') {
                this.crossBSelected = true
            }else if (cross === 'C') {
                this.crossBSelected = true
            }else if (cross === 'D') {
                this.crossBSelected = true
            }else if (cross === 'E') {
                this.crossBSelected = true
            }else if (cross === 'F') {
                this.crossBSelected = true
            }else if (cross === 'G') {
                this.crossBSelected = true
            }else if (cross === 'H') {
                this.crossBSelected = true
            }
        }
    }
}
</script>
