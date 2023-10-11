<template>
  <section class="footer">
    <p>© DUGIMAIL. All rights reserved.</p>
    <p>
      If you have any questions please contact us
      <a href="mailto:your.email@example.com">Shahribonu@outlook.com</a>
    </p>
    <div class="icons">
      <img src="../assets/images/icon1.png" alt="icon1" />
      <img src="../assets/images/icon2.png" alt="icon1" />
      <img src="../assets/images/icon3.png" alt="icon1" />
      <img src="../assets/images/icon4.png" alt="icon1" />
      <img src="../assets/images/icon5.png" alt="icon1" />
    </div>
  </section>
</template>

<style scoped>
.footer {
  height: 160px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100%;
  padding: 24px;
  border-top: 2px solid #6c6e72;
  border-width: 90% auto;
}
p {
  font-size: 18px;
  color: #525f7f;
  margin: 10px 0;
  text-align: center;
}
a {
  text-decoration: none;
  color: #7b93cb;
}
.icons {
  display: flex;
}
img {
  margin: 10px;
  width: 20px;
}
</style>
