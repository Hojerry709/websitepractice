<template>
  <section class="treeline">
    <div class="lines-top">
      <span class="tline middle"></span>
      <span class="tline"></span>
      <span class="tline"></span>
    </div>
    <div class="text">
      <span class="line"></span>
      <div class="text-block">
        <h2>All Natural Ingredients</h2>
        <p>Believing that quality will foster radiance and inspire an overall sense of well-being</p>
      </div>
      <span class="line"></span>
    </div>
  </section>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Marcellus+SC&family=Mukta+Vaani:wght@200;300;400;500;600;700;800&display=swap');

.treeline {
  text-align: center;
  padding: 60px 20px;
  max-width: 1600px;
  margin: 0 auto;
}

.lines-top {
  display: flex;
  justify-content: center;
  gap: 10px;
  margin-top: -30px;
}

.tline {
  width: 40px;
  height: 2px;
  background-color: #C5B0AA;
}

.tline.middle {
  background-color: #59260B;
}

.text {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 20px;
  color: #59260B;
  margin-top: -50px;
  flex-wrap: wrap;
}

.line {
  width: 2px;
  height: 220px;
  background-color: #C5B0AA;
  margin-top: 100px;
}

.text-block {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 50px;
  max-width: 800px;
}

h2 {
  font-size: 60px;
  color: #59260B;
  font-family: 'Marcellus SC', serif;
  white-space: nowrap;
  margin-bottom: 8px;
}

p {
  font-size: 28px;
  color: #59260B;
  margin: 0;
  font-family: 'Mukta Vaani', sans-serif;
  text-align: center;
  max-width: 750px;
  margin-top: 20px;
}

@media (max-width: 1024px) {
  .text {
    gap: 10px;
  }

  .line {
    height: 180px;
    margin-top: 50px;
  }

  h2 {
    font-size: 48px;
  }

  p {
    font-size: 24px;
    max-width: 90%;
  }
}

@media (max-width: 768px) {
  .text {
    flex-direction: column;
    align-items: center;
  }

  .line {
    display: none;
  }

  h2 {
    font-size: 36px;
  }

  p {
    font-size: 20px;
    max-width: 100%;
  }
}
</style>
