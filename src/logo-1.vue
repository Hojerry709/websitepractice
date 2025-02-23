<template>
  <footer class="footer">
    <div class="container">
      <div class="flogo">
        <img src="/public/Vector (1).png" alt="Logo" />
      </div>
      <div class="content">
        <div class="column products">
          <h3>Products</h3>
          <ul>
            <li>Solid perfume</li>
            <li>Scented Ovals</li>
            <li>Scented Candles</li>
          </ul>
        </div>
        <div class="column">
          <h3>About us</h3>
          <ul>
            <li>Our story</li>
            <li>Blog</li>
            <li>Contacts</li>
          </ul>
        </div>
        <div class="column">
          <h3>Social</h3>
          <ul>
            <li>Instagram</li>
            <li>Twitter</li>
            <li>Facebook</li>
          </ul>
        </div>
        <div class="contact">
          <p>60 Midway Road, Suite 12</p>
          <p>Green Bay WI 54280</p>
          <p>401-280-4690</p>
        </div>
      </div>
    </div>
    <p class="year">© 2022 SV Shop. All rights reserved.</p>
  </footer>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Marcellus+SC&family=Mukta+Vaani:wght@200;300;400;500;600;700;800&display=swap');

.footer {
  background: #59260B;
  color: #fff;
  padding: 40px 60px;
  text-align: center;
}

.container {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
}

.flogo {
  display: flex;
  align-items: center;
  height: 100%;
}

.flogo img {
  width: 40px;
}

.content {
  display: flex;
  justify-content: space-between;
  flex-grow: 1;
  text-align: left;
}

.column {
  margin: 0 30px;
}

.products {
  margin-left: 50px;
}

.column h3 {
  font-size: 16px;
  margin-bottom: 10px;
  font-family: Mukta Vaani;
}

.column ul {
  list-style: none;
  padding: 0;
}

.column ul li {
  margin-bottom: 8px;
  font-family: Mukta Vaani;
}

.column ul li a {
  color: #ffff;
  text-decoration: none;
  transition: 0.3s;
}

.column ul li a:hover {
  text-decoration: underline;
}

.contact {
  text-align: right;
  font-size: 14px;
  font-family: Mukta Vaani;
}

.year {
  margin-top: 20px;
  font-size: 14px;
  text-align: center;
  font-family: Mukta Vaani;
}

</style>
