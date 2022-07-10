<template>
  <div class='home'>
    <div class='center'>
      <h1 class='title'>TrainFormuls</h1>
      <h3 class='motto'>everything you need for a successful study of physics</h3>
      <div class='buttons'>
        <Button text='Let`s start!' color='#fa6400' hover='#fb8332' active='#c85000' route='test'></Button>
        <Button text='Learn more' color='#fa6400' hover='#fb8332' active='#c85000' route='about'></Button>
        <!-- change color of second button -->
      </div>
    </div>
  </div>
</template>

<script>
import Button from '@/components/Shared/Button.vue'

export default {
  data() {
    return {

    }
  },
  components: {
    Button
  }
}
</script>

<style scoped>
.home {
  width: 100%;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
.title {
  font-family: 'OswaldMedium';
  font-style: normal;
  font-weight: 500;
  font-size: 48px;
  line-height: 71px;
  text-align: center;
  letter-spacing: 0.02em;
}
.motto {
  font-family: 'OswaldMedium';
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  line-height: 27px;
  text-align: center;
  text-transform: uppercase;
}
.buttons {
  width: 100%;
  height: 10vh;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>
