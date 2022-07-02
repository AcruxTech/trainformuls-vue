<template>
  <router-view/>
  <span class='author'><a href='https://github.com/AcruxTech'>powered by AcruxTech</a></span>
</template>

<style>
@font-face {
  font-family: 'OswaldMedium'; 
  src: url('assets/fonts/Oswald-Medium.ttf') format('truetype'); 
  font-style: normal; 
  font-weight: normal; 
} 
@font-face {
  font-family: 'OswaldRegular'; 
  src: url('assets/fonts/Oswald-Regular.ttf') format('truetype'); 
  font-style: normal; 
  font-weight: normal; 
} 
@font-face {
  font-family: 'OpenSansRegular'; 
  src: url('assets/fonts/OpenSans-Regular.ttf') format('truetype'); 
  font-style: normal; 
  font-weight: normal; 
} 
@font-face {
  font-family: 'SyneMedium'; 
  src: url('assets/fonts/Syne-Medium.ttf') format('truetype'); 
  font-style: normal; 
  font-weight: normal; 
} 
@font-face {
  font-family: 'SyneRegular'; 
  src: url('assets/fonts/Syne-Regular.ttf') format('truetype'); 
  font-style: normal; 
  font-weight: normal; 
} 

#app {
  background: rgb(255,171,44);
  background: linear-gradient(166deg, rgba(255,171,44,1) 0%, rgba(25,25,25,1) 100%);
}

.author {
  position: absolute;
  bottom: 50px;
  right: 50px;
  font-family: 'OpenSansRegular';
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 22px;
}
.author > a,
.author > a:visited {
  text-decoration: none;
  color: #fff;
}
.author > a:hover {
  text-decoration: underline;
}
</style>
