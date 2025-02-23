<template>
  <div class="container">
    <h1 class="title">Read our Blog</h1>
    <div class="blog-layout">
      <div class="card big">
        <img src="/public/7b67cedeabed2083caa3eaa7b86f0587.jpg" alt="Candle" />
        <div class="overlay">
          <p>Our Charity Mission</p>
        </div>
      </div>
      <div class="right-section">
        <div class="top-row">
          <div class="card medium">
            <img src="/public/d46e5fa2139ec04531993a23fd1530d7.jpg" alt="Solid Soap" />
            <div class="overlay">
              <p>Why Solid?</p>
            </div>
          </div>
          <div class="card small">
            <img src="/public/0dcee9257b82ae5e67ea8a977dec09dc.jpg" alt="POV" />
            <div class="overlay">
              <p>POV</p>
            </div>
          </div>
        </div>
        <button class="read-more">Read more in our Blog</button>
        <div class="card wide">
          <img src="/public/d041eb0ea9fdcdc2afcb8e82e8ea2180.jpg" alt="Sustainable Practice" />
          <div class="overlay">
            <p>Our Sustainable Practice</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Marcellus+SC&family=Mukta+Vaani:wght@200;300;400;500;600;700;800&display=swap');

.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

.title {
  font-size: 48px;
  font-family: Marcellus SC;
  margin-bottom: 20px;
}

.blog-layout {
  display: flex;
  justify-content: center;
  gap: 20px;
  max-width: 1200px;
}

.card {
  position: relative;
  border: 2px solid #59260B;
  display: flex;
  flex-direction: column;
  align-items: center;
  overflow: hidden;
  background: white;
}

.card img {
  width: 100%;
  height: auto;
  object-fit: cover;
}

.overlay {
  position: absolute;
  bottom: 0;
  width: 100%;
  background: #EDEBE8;
  color: #000000;
  text-align: center;
  padding: 10px 0;
  font-family: Mukta Vaani;
  font-size: 17px;
}

.big {
  width: 490px;
  height: 700px;
}

.right-section {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.top-row {
  display: flex;
  gap: 10px;
}

.medium {
  width: 282px;
  height: 400px;
}

.small {
  width: 386px;
  height: 316px;
}

.read-more {
  position: relative;
  right: -150px;
  width: 386px;
  height: 54px;
  background: #59260B;
  color: white;
  border: none;
  margin-top: -55px;
}

.wide {
  width: 698px;
  height: 270px;
  margin-top: 25px;
}

@media (max-width: 1024px) {
  .blog-layout {
    grid-template-columns: 1fr;
  }

  .big {
    height: 600px;
  }

  .medium {
    height: 350px;
  }

  .small {
    height: 280px;
  }

  .wide {
    height: 220px;
  }

  .read-more {
    max-width: 100%;
  }
}

@media (max-width: 768px) {
  .title {
    font-size: 36px;
  }

  .big {
    height: 500px;
  }

  .top-row {
    grid-template-columns: 1fr;
  }

  .medium, .small, .wide {
    height: auto;
  }

  .read-more {
    font-size: 14px;
    height: 48px;
  }
}
</style>
