<template>
  <header class="header">
    <div class="wrapper">
      <div class="left">
        <span class="text">Solid Parfume</span>
        <span class="text">Scented Ovals</span>
        <span class="text">Scented Candles</span>
      </div>
      <div class="center">
        <img src="/public/Vector123.png" alt="logo" class="logo" />
      </div>
      <div class="right">
        <img src="/public/user_icn.png" alt="Icon 1" class="icon" />
        <img src="/public/Vector.png" alt="Icon 2" class="icon" />
        <img src="/public/cart_icn.png" alt="Icon 3" class="icon" />
      </div>
    </div>
  </header>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Marcellus+SC&family=Mukta+Vaani:wght@200;300;400;500;600;700;800&display=swap');

.header {
  width: 100%;
  background-color: #ffffff;
  border-bottom: 1px solid #ddd;
  padding: 15px 0;
}

.wrapper {
  max-width: 1600px;
  width: 100%;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 20px;
}

.left {
  display: flex;
  gap: 20px;
  padding-left: 8%;
  margin: 0 auto;
}

.text {
  font-size: 17px;
  color: black;
  font-family: 'Mukta Vaani', sans-serif;
}

.center {
  flex-grow: 1;
  display: flex;
  justify-content: center;
}

.logo {
  position: relative;
  width: 40px;
  height: 40px;
  left: -150px;
}

.right {
  display: flex;
  gap: 15px;
  align-items: center;
}

.icon {
  width: 20px;
  height: 20px;
}

@media (max-width: 1024px) {
  .wrapper {
    padding: 0 10px;
  }

  .left {
    gap: 10px;
  }

  .text {
    font-size: 15px;
  }

  .logo {
    width: 40px;
    height: 40px;
  }

  .icon {
    width: 18px;
    height: 18px;
  }
}

@media (max-width: 600px) {
  .wrapper {
    flex-direction: column;
    align-items: center;
    text-align: center;
  }

  .left {
    flex-direction: column;
    gap: 5px;
  }

  .text {
    font-size: 14px;
  }

  .logo {
    width: 35px;
    height: 35px;
  }

  .right {
    margin-top: 10px;
  }

  .icon {
    width: 16px;
    height: 16px;
  }
}
</style>
