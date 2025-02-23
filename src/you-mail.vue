<template>
  <div class="popular-flavors">
    <h2 class="title">You may also like</h2>
    <div class="slider-container">
      <button @click="prevSlide" class="arrow left-arrow">&lt;</button>
      <div class="card-container">
        <div v-for="(item, index) in items" :key="index" :class="['card', { 'gray-card': index === 2 }]">
          <img :src="item.heartIcon" alt="Heart Icon" class="heart-icon" />
          <img :src="item.image" alt="Product Image" class="card-image" />
          <div class="card-content">
            <h3 class="card-title">{{ item.title }}</h3>
            <p class="card-subtitle">{{ item.subtitle }}</p>
            <p class="card-price">{{ item.price }}</p>
          </div>
        </div>
      </div>
      <button @click="nextSlide" class="arrow right-arrow">&gt;</button>
    </div>
  </div>

  <section class="treeline">
    <div class="lines-top">
      <span class="tline middle"></span>
      <span class="tline"></span>
      <span class="tline"></span>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          image: "/photo (7).png",
          heartIcon: "/heart_icn.png",
          title: "Rose Frankincense & Patchouli",
          subtitle: "Scented Candle",
          price: "$105.00",
        },
        {
          image: "/photo (6).png",
          heartIcon: "/heart_icn (1).png",
          title: "Rose Frankincense & Patchouli",
          subtitle: "Scented Candle",
          price: "$105.00",
        },
        {
          image: "/photo (4).png",
          heartIcon: "/heart_icn (2).png",
          title: "Rose Frankincense & Patchouli",
          subtitle: "Scented Candle",
          price: "$105.00",
        },
        {
          image: "/photo (3).png",
          heartIcon: "/heart_icn (2).png",
          title: "Rose Frankincense & Patchouli",
          subtitle: "Scented Candle",
          price: "$105.00",
        },
      ],
    };
  },
  methods: {
    prevSlide() {
      console.log("Previous slide");
    },
    nextSlide() {
      console.log("Next slide");
    },
  },
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Marcellus+SC&family=Mukta+Vaani:wght@200;300;400;500;600;700;800&display=swap');

.popular-flavors {
  background: linear-gradient(to bottom, #EDEBE8 80%, white 20%);
  padding: 40px 0;
  text-align: center;
}

.title {
  font-size: 48px;
  font-weight: bold;
  margin-bottom: 50px;
  font-family: 'Marcellus SC', serif;
}

.slider-container {
  max-width: 1600px;
  width: 100%;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
}

.card-container {
  display: flex;
  justify-content: center;
  gap: 20px;
  flex-wrap: wrap;
}

.card {
  width: 280px;
  height: 350px;
  background-color: #ffffff;
  border: 2px solid #C5B0AA;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 10px;
  position: relative;
}

.gray-card {
  background-color: #EDEBE8;
  border: 2px solid #59260B;
}

.card-image {
  width: 100%;
  height: 60%;
  object-fit: cover;
}

.card-content {
  padding: 10px;
  text-align: center;
  font-family: 'Mukta Vaani', sans-serif;
}

.card-title {
  font-size: 16px;
  font-weight: bold;
  margin: 10px 0;
}

.card-subtitle {
  font-size: 14px;
  color: #000;
}

.card-price {
  font-size: 14px;
  margin-top: 8px;
}

.heart-icon {
  position: absolute;
  top: 8px;
  right: 8px;
  width: 15px;
  height: 15px;
  cursor: pointer;
}

.arrow {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  background: none;
  border: none;
  font-size: 32px;
  cursor: pointer;
  padding: 10px;
}

.left-arrow {
  left: -60px;
}

.right-arrow {
  right: -60px;
}

.treeline {
  text-align: center;
  padding: 60px 20px;
  position: relative;
}

.lines-top {
  display: flex;
  justify-content: center;
  gap: 10px;
  margin-top: -60px;
}

.tline {
  width: 40px;
  height: 2px;
  background-color: #C5B0AA;
}

.tline.middle {
  width: 40px;
  height: 2px;
  background-color: #59260B;
}

@media (max-width: 1024px) {
  .title {
    font-size: 40px;
  }

  .card-container {
    flex-wrap: wrap;
    justify-content: center;
  }

  .card {
    width: 250px;
    height: 320px;
  }

  .card-title {
    font-size: 14px;
  }

  .card-subtitle,
  .card-price {
    font-size: 12px;
  }

  .left-arrow {
    left: -40px;
  }

  .right-arrow {
    right: -40px;
  }
}

@media (max-width: 768px) {
  .title {
    font-size: 32px;
  }

  .card-container {
    gap: 10px;
  }

  .card {
    width: 220px;
    height: 300px;
  }

  .card-title {
    font-size: 14px;
  }

  .card-subtitle,
  .card-price {
    font-size: 12px;
  }

  .arrow {
    font-size: 28px;
  }

  .left-arrow {
    left: -20px;
  }

  .right-arrow {
    right: -20px;
  }
}
</style>
