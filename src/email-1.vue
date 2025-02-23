<template>
  <div class="wrapper">
    <div class="container">
      <div class="image-container">
        <img src="/public/7242a592a357888d5258cfec441b158a.jpg" alt="Decorative" class="styled-image" />
      </div>
      <div class="form-container">
        <h1>Get in Touch</h1>
        <p>
          Get daily expert perfume tips, special temporal promotions and an extra
          discount for internet payments.
        </p>
        <input type="email" placeholder="Enter your email" />
        <p class="terms">
          By clicking OK, I agree to the
          Terms and Conditions and the
          Privacy Policy.
        </p>
        <button>Submit</button>
      </div>
    </div>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Marcellus+SC&family=Mukta+Vaani:wght@200;300;400;500;600;700;800&display=swap');

.wrapper {
  max-width: 1600px;
  width: 100%;
  margin: 0 auto;
}

.container {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
  gap: 40px;
  background: #fff;
  padding: 40px;
}

.image-container {
  width: 300px;
  height: 300px;
  overflow: hidden;
  display: flex;
  justify-content: center;
  align-items: center;
}

.styled-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 0 50% 50% 50%;
}

.form-container {
  max-width: 600px;
  flex: 1;
}

h1 {
  font-size: 48px;
  font-family: 'Marcellus SC', serif;
  color: #59260B;
}

p {
  font-size: 17px;
  color: #000000;
  font-family: 'Mukta Vaani', sans-serif;
}

input {
  width: 100%;
  padding: 10px;
  margin: 10px 0;
  border: none;
  border-bottom: 2px solid #59260B;
  outline: none;
  background: transparent;
}

.terms {
  font-size: 15px;
  color: #000000;
  font-family: 'Mukta Vaani', sans-serif;
}

button {
  padding: 10px 20px;
  background: #EDEBE8;
  color: black;
  border: 1px solid #59260B;
  cursor: pointer;
  border-radius: 0;
}

@media (max-width: 1024px) {
  .container {
    flex-direction: column;
    text-align: center;
  }

  .image-container {
    width: 250px;
    height: 250px;
  }

  h1 {
    font-size: 36px;
  }

  p {
    font-size: 16px;
  }
}

@media (max-width: 600px) {
  .wrapper {
    max-width: 100%;
    padding: 0 20px;
  }

  .container {
    padding: 20px;
  }

  .image-container {
    width: 200px;
    height: 200px;
  }

  h1 {
    font-size: 28px;
  }

  p, .terms {
    font-size: 14px;
  }

  input {
    font-size: 14px;
    padding: 8px;
  }

  button {
    padding: 8px 16px;
    font-size: 14px;
  }
}
</style>
