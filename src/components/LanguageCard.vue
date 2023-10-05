<template>
  <div class="animation-container">
    <div
        class="card_languages"
        v-for="(imgSrc, index) in arrayImg"
        :key="index"
        :style="{ transform: `translateX(${translateX}px)` }"
    >
      <img :src="imgSrc" alt="image">
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      arrayImg: [
        "/src/assets/swift.png",
        "/src/assets/swiftui.png",
        "/src/assets/java.png",
        "/src/assets/vue.png",
        "/src/assets/firebase.png",
        "/src/assets/realm.png",
        "/src/assets/graphql.png",
      ],
      cardWidth: 95, // Ширина карточки
      translateX: 0, // Начальное положение
      direction: 1, // Начальное направление анимации
      animationInterval: null, // Интервал анимации
    };
  },
  mounted() {
    this.startAnimation();
  },
  methods: {
    startAnimation() {
      if (this.animationInterval) {
        clearInterval(this.animationInterval);
      }
      this.animationInterval = setInterval(() => {
        this.translateX += 2 * this.direction;
        if (
            this.direction === 1 &&
            this.translateX >= window.innerWidth - this.cardWidth
        ) {
          this.direction = -1; // Изменяем направление на обратное
        } else if (this.direction === -1 && this.translateX <= -this.cardWidth) {
          this.direction = 1; // Возвращаем картинку за пределы экрана слева
        }
      }, 30);
    },
  },
};
</script>

<style>
.animation-container {
  overflow: hidden;
  display: flex;
  margin: 100px;
}

.card_languages {
  width: 95px;
  height: 95px;
  flex-shrink: 0;
  border-radius: 40px;
  background-color: #1e311c;
  display: flex;
  margin: 10px;
  transition: transform 0.2s ease;
}

.card_languages img {
  width: 75px;
  height: 75px;
  margin: 10px;
  border-radius: 20px;
}
</style>
