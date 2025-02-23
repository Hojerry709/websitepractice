<template>
  <section class="categories">
    <h2 class="main-title">Shop by categories</h2>
    <div class="products-grid">
      <div class="product-card solid-parfume">
        <div class="product-title">Solid Parfume</div>
        <img src="/d476154beb25fb4ea8d8c834e91e82ad.jpg" alt="Solid Perfume" />
      </div>
      <div class="product-card scented-ovals">
        <div class="product-title">Scented Ovals</div>
        <img src="/01cb53be7ae57720b9cb0617cbd1b53a.jpg" alt="Scented Ovals" />
      </div>
      <div class="product-card scented-candles">
        <div class="product-title dark-title">Scented Candles</div>
        <img src="/c37beb7d1b619f03612eefdd707d58c9.jpg" alt="Scented Candles" />
      </div>
    </div>
  </section>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Marcellus+SC&family=Mukta+Vaani:wght@200;300;400;500;600;700;800&display=swap');

.categories {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  padding: 50px 20px;
}

.main-title {
  margin-bottom: 20px;
  font-size: 24px;
  font-family: Marcellus SC;
}

.products-grid {
  display: grid;
  grid-template-columns: 594px 594px;
  grid-template-rows: 400px 400px;
  grid-template-areas:
    "solid-parfume scented-candles"
    "scented-ovals scented-candles";
  gap: 10px;
  max-width: 1200px;
  margin: 0 auto;
}

.product-card {
  position: relative;
  overflow: hidden;
  border: 2px solid #59260B;
  font-family: Mukta Vaani;
}

.solid-parfume {
  grid-area: solid-parfume;
  width: 594px;
  height: 400px;
  background-color: #EDEBE8;
}

.scented-ovals {
  grid-area: scented-ovals;
  width: 594px;
  height: 400px;
  background-color: #EDEBE8;
}

.scented-candles {
  grid-area: scented-candles;
  width: 594px;
  height: 810px;
  background-color: #59260B;
}

.product-card img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.product-title {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  background-color: #EDEBE8;
  text-align: center;
  font-size: 15px;
  font-family: Mukta Vaani;
  padding: 10px;
  z-index: 10;
}

.dark-title {
  background-color: #59260B;
  color: #FFFFFF;
}

@media (max-width: 1024px) {
  .products-grid {
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  }

  .scented-candles {
    height: 500px;
  }

  .main-title {
    font-size: 28px;
  }
}

@media (max-width: 768px) {
  .products-grid {
    grid-template-columns: 1fr;
  }

  .scented-candles {
    height: 400px;
  }

  .main-title {
    font-size: 24px;
  }

  .product-title {
    font-size: 16px;
    padding: 10px;
  }
}
</style>
