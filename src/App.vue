<template>
  <h1>
    <a href="https://github.com/phyark"><span class="i-text">I</span>n96</a>
  </h1>
  <span class="fixRightBottom">phyark</span>
</template>

<style scoped>
h1 {
  font-size: 10em;
  color: #ffffff;
  font-family: fantasy, Arial, "Helvetica Neue", Helvetica, sans-serif;
  cursor: default;
  position: relative;
}

a {
  color: #f1f1f1;
  position: relative;
  z-index: 1;
  user-select: none;
}
h1::after {
  position: absolute;
  bottom: -20%;
  left: 0;
  display: inline-block;
  content: '';
  width: 100%;
  height: 0.3em;
  background: #df9138;
  border-radius: 6px 9px 90px 90px;
  z-index: 0;
  transition: .3s ease .1s;
}

h1::after:hover {
  bottom: 12px;
  ;
}

.i-text {
  font-size: 0.8em;
  position: relative;
}

.i-text::before {
  position: absolute;
  display: inline-block;
  content: '';
  width: 0.4em;
  height: 0.29em;
  background-color: orange;
  left: calc((100% - 0.4em) / 2);
  border-radius: 0 50% 50%;
  transform: rotate(80deg);
  animation: myFrame 1s linear infinite;
}
.fixRightBottom {
  position: fixed;
  bottom: 20px;
  right: 20px;
  font-size: 2em;
  font-family: fantasy;
}

@keyframes myFrame {
  0% {
    transform: rotate(80deg);
    width: 0.4em;
    height: 0.29em;
  }

  25% {
    transform: rotate(90deg);
    width: 0.4em;
    height: 0.26em;
  }

  50% {
    transform: rotate(92deg);
    width: 0.4em;
    height: 0.20em;
  }

  75% {
    transform: rotate(78deg);
    width: 0.4em;
    height: 0.26em;
  }

  75% {
    transform: rotate(80deg);
    width: 0.4em;
    height: 0.29em;
  }
}
</style>
