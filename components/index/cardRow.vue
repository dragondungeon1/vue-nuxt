<template>
  <section>
    <b-container class="bv-example-row mb-3">
      <b-row cols="3, 1" >
        <b-col class="text-white">
          <div class="card text-center">
            <p class="card-head">About</p>
            <hr class="solid" />
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis
              nihil magni voluptatem totam nihil magni voluptatem totamnihil
              magni voluptatem
            </p>
            <a class="btn btn-outline-primary" href="/about">Learn more</a>
          </div>
        </b-col>

        <b-col class="text-white mb-5"
          ><div class="card text-center">
            <p class="card-head">Services</p>
            <hr class="solid" />
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis
              nihil magni voluptatem totam nihil magni voluptatem totamnihil
              magni voluptatem
            </p>
            <a class="btn btn-outline-primary" href="#">Learn more</a>
          </div>
        </b-col>

        <b-col class="text-white">
          <div class="card text-center">
            <p class="card-head">Contact</p>
            <hr class="solid" />
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis
              nihil magni voluptatem totam nihil magni voluptatem totamnihil
              magni voluptatem
            </p>
            <a class="btn btn-outline-primary" href="#">Learn more</a>
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

.card-head{
  font-weight: 400;
  font-size: 19px;
  }

p {
  font-weight: 100;
}

.card {
  background-color: transparent;
}

section{
  margin-bottom: 3rem;
}
</style>
