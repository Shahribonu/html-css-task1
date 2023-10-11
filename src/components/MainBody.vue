<template>
  <div class="main">
    <h1>Popular Wordpress plugins</h1>
    <div class="cards">
      <div class="card" v-for="element in elements" key="element.text">
        <img src="../assets/images/image1.png" alt="" />
        <div class="content">
          <h2 class="text">{{ element.text }}</h2>
          <p class="price">{{ element.price }}</p>
          <button>Buy</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const elements = [
  { img: "../assets/images/image1.png", text: "RubIcon", price: "$100" },
  { img: "../assets/images/image1.png", text: "Camera", price: "$200" },
  { img: "../assets/images/image1.png", text: "Generator", price: "$100" },
  { img: "../assets/images/image1.png", text: "InvoiceCreator", price: "$300" },
];
</script>

<style scoped>
.main {
  display: flex;
  flex-direction: column;
  width: 100%;
  padding: 24px;
}
.cards {
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
  margin-bottom: 20px;
  align-content: stretch;
}
.card {
  width: 310px;
}
.content {
  padding: 0 10px 5px;
  margin-top: -35px;
}
h1 {
  font-weight: normal;
}
h2 {
  font-size: 25px;
  color: #484848;
  font-family: Poppins;
}
p {
  color: #489dff;
  font-weight: 500;
  font-size: 18px;
  padding: 5px 0;
}
button {
  background-color: #489dff;
  padding: 15px 50px;
  color: #fff;
  border-radius: 10px;
  outline: none;
  border: none;
  font-size: 18px;
  margin: 10px 0;
}
@media screen and (max-width: 687px) {
  .card {
    width: 100%;
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
  }
  h1 {
    text-align: center;
  }
  .content {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
  }
}
</style>
