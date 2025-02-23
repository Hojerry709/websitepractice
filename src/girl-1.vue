<template>
  <section class="text">
    <div class="wrapper">
      <div class="text-container">
        <div class="l-text">
          <h2>Solid Parfume and scented candles for cozy home</h2>
          <button class="shop-button">Shop Now</button>
        </div>
        <div class="foto">
          <img src="/public/photo.png" alt="fotogirl" class="foto-girl"/>
          <img src="/public/photo (1).png" alt="fotofigura" class="foto-figura" />
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Marcellus+SC&family=Mukta+Vaani:wght@200;300;400;500;600;700;800&display=swap');

.text {
  width: 100%;
  background-color: #EDEBE8;
  padding: 60px 0;
}

.wrapper {
  max-width: 1600px;
  width: 100%;
  margin: 0 auto;
  padding: 0 20px;
}

.text-container {
  max-width: 1200px;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 50px;
  padding: 0 20px;
}

.l-text {
  position: relative;
  right: 80px;
  max-width: 1000px;
  width: 500px;
  font-family: Marcellus SC;
  color: #59260B;
  bottom: 100px;
  font-size: 33px;
}

.shop-button {
  background-color: #59260B;
  color: white;
  border: none;
  height: 54px;
  width: 178px;
  padding: 17px 30px;
  cursor: pointer;
  font-family: 'Mukta Vaani', sans-serif;
}

.foto {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
}

.foto-girl {
  width: 700px;
  height: auto;
  position: relative;
  right: -200px;
  bottom: 20px;
  overflow: hidden;
}

.foto-figura {
  position: absolute;
  bottom: -15px;
  right: 400px;
  width: 400px;
}

@media (max-width: 1024px) {
  .text-container {
    flex-direction: column;
    text-align: center;
  }

  .l-text {
    font-size: 28px;
    text-align: center;
  }

  .shop-button {
    width: 150px;
    height: 50px;
    font-size: 16px;
  }

  .foto-girl {
    max-width: 500px;
  }

  .foto-figura {
    width: 300px;
    right: 5%;
  }
}

@media (max-width: 600px) {
  .wrapper {
    padding: 0 10px;
  }

  .l-text {
    font-size: 24px;
  }

  .shop-button {
    width: 140px;
    height: 45px;
    font-size: 14px;
  }

  .foto-girl {
    max-width: 300px;
  }

  .foto-figura {
    width: 200px;
    right: 0;
  }
}
</style>
