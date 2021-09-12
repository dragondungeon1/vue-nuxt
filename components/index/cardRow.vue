<template>
  <section>
    <b-container class="bv-example-row mb-3">
      <b-row cols="3">
        <b-col class="text-white">
          <div class="card text-center">
            <h4>About</h4>
            <hr class="solid" />
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis
              nihil magni voluptatem totam nihil magni voluptatem totamnihil
              magni voluptatem
            </p>
            <a class="btn text-white btn-outline" href="/about">Learn more</a>
          </div>
        </b-col>

        <b-col class="text-white mb-5"
          ><div class="card text-center">
            <h4>Services</h4>
            <hr class="solid" />
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis
              nihil magni voluptatem totam nihil magni voluptatem totamnihil
              magni voluptatem
            </p>
            <a class="btn text-white btn-outline" href="#">Learn more</a>
          </div>
        </b-col>

        <b-col class="text-white">
          <div class="card text-center">
            <h4>Contact</h4>
            <hr class="solid" />
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis
              nihil magni voluptatem totam nihil magni voluptatem totamnihil
              magni voluptatem
            </p>
            <a class="btn text-white btn-outline" href="#">Learn more</a>
          </div></b-col
        >
      </b-row>
    </b-container>
  </section>
</template>

<style lang="css" scoped>
hr.solid {
  border-top: 1px solid #5c7ae4;
  opacity: 50%;
}

h4 {
  font-weight: 400;
  font-size: 22px;
}

p {
  font-weight: 100;
}

.card {
  background-color: transparent;
}

.btn {
  background-color: #5c7ae4;
}
.btn:hover {
  background-color: transparent;
  color: white;
  border: 1px solid #5c7ae4;
}
section{
  margin-bottom: 3rem;
}
</style>
