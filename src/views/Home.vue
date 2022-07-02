<template>
  <div class='home'>
    <div class='center'>
      <h1 class='title'>TrainFormuls</h1>
      <h3 class='motto'>everything you need for a successful study of physics</h3>
      <div class='buttons'>
        <button type='button' class='button start'>Let`s start!</button>
        <button type='button' class='button more'>Learn more</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {

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
  width: 30vw;
  height: 10vh;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.button {
  width: 40%;
  height: 50%;
  border: none;
  border-radius: 15px;
  outline: none;
}
.start {
  background-color: #057D9F;
}
</style>
