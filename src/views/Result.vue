<template>
  <div class='result'>
    <div class='center'>
      <div class='info margin'>
        <h1 class='title'>Your result:</h1>
        <h1 class='points'>98 points (max: 100)</h1>
      </div>
      <div class='copy-link margin'>
        <label class='text'>Share your result with friends: </label>
        <input type='text' class='copy-link-input' value='https://github.com' readonly>
        <button type='button' class='copy-link-button'></button>
      </div>
      <Button color='#fa6400' hover='#fb8332' active='#c85000' route='test'>Try again</Button>
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
.result {
  width: 100%;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
.center {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.title {
  font-family: 'OswaldMedium';
  font-style: normal;
  font-weight: 500;
  font-size: 36px;
  line-height: 53px;
  text-align: center;
  letter-spacing: 0.02em;
}
.points {
  font-family: 'OswaldMedium';
  font-style: normal;
  font-weight: 400;
  font-size: 40px;
  line-height: 60px;
  text-align: center;
  text-transform: uppercase;
}
.text {
  font-family: 'OpenSansRegular';
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 22px;
}
.copy-link {
  width: 100%;
  height: 4vh;
  display: flex;
  align-items: center;
}
.copy-link-input {
  height: 4vh;
  flex-grow: 1;
  padding: 0 8px;
  font-size: 14px;
  border: 1px solid #cccccc;
  border-right: none;
  outline: none;
}
.copy-link-input:hover {
  background: #eee;
}
.copy-link-button {
  flex-shrink: 0;
  width: 4vh;
  height: 4vh;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #dddddd;
  color: #333;
  outline: none;
  border: 1px solid #cccccc;
  cursor: pointer;
}
.copy-link-button:hover {
  background: #ccc;
}
.margin {
  margin-bottom: 5vh;
}
</style>
