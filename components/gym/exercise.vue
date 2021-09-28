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
        v-for="(check, index) in checks"
        :key="`check_${index}`"
        class="item border-white text-white"
        :class="{
          'item--success': isChecked(index) === true,
          'item--failed': isChecked(index) === false
        }"
      >
        <i @click="toggleCheck(index, true)" class="fas fa-check fa-3x"></i>
        <div>{{ check.name }}</div>
        <div>{{check.weight}}</div>
        <div>
          <i @click="toggleCheck(index, false)" class="fas fa-times fa-3x"></i>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      checks: [
        {
          name: 'bench press',
          weight: '3x10x70' ,
        },
        {
          name: 'Cardio'
        }
      ],
      checklist: []
    };
  },
  methods: {
    toggleCheck(check, state) {
      const index = this.checklist.findIndex((item) => item.number === check);

      // Add item that is not already present in the checklist
      if (index === -1) {
        this.checklist.push({
          number: check,
          state
        });

        return;
      }

      // Remove item when state is equal
      if (this.checklist[index].state === state) {
        this.checklist.splice(index, 1);

        return;
      }

      // switch from one state to another
      Object.assign(this.checklist[index], { state });
    },
    isChecked(check) {
      const item = this.checklist.find((item) => item.number === check);

      // If item is not known, return
      if (typeof item === 'undefined') {
        return;
      }

      // Check if state is true
      return item.state === true;
    }
  },
};
</script>

<style lang="css" scoped>
.item {
  width: 100%;
  display: flex;
  justify-content: space-between;
  border: 1px solid white;
  border-radius: 3px;
  padding: 3%;
  background: transparent;
}

.item.item--success {
  background: green;
}

.item.item--failed {
  background: red;
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
