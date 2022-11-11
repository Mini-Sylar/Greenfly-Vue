<template lang="">
  <div>
    <nav>
      <div class="logo">
        <img src="@/assets/images/logo.png" alt="" />
      </div>
      <div id="nav-icon1" class="hamburger">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </nav>
  </div>
</template>
<script>
export default {
    data() {
        return {

        }
    },
};
</script>
<style scoped>
/* Ham */
#nav-icon1 {
    display: block;
    width: 50px;
    height: 45px;
    position: absolute;
    margin: 20px auto;
    -webkit-transform: rotate(0deg);
    -moz-transform: rotate(0deg);
    -o-transform: rotate(0deg);
    transform: rotate(0deg);
    -webkit-transition: 0.5s ease-in-out;
    -moz-transition: 0.5s ease-in-out;
    -o-transition: 0.5s ease-in-out;
    transition: 0.5s ease-in-out;
    cursor: pointer;
    right: 5%;
    z-index: 25;
}

#nav-icon1 span {
    display: block;
    position: absolute;
    height: 3px;
    width: 90%;
    background: var(--accent-color);
    border-radius: 9px;
    opacity: 1;
    left: 0;
    -webkit-transform: rotate(0deg);
    -moz-transform: rotate(0deg);
    -o-transform: rotate(0deg);
    transform: rotate(0deg);
    -webkit-transition: 0.25s ease-in-out;
    -moz-transition: 0.25s ease-in-out;
    -o-transition: 0.25s ease-in-out;
    transition: 0.25s ease-in-out;
}

#nav-icon1 span:nth-child(1) {
    top: 0px;
}

#nav-icon1 span:nth-child(2) {
    top: 12px;
}

#nav-icon1 span:nth-child(3) {
    top: 24px;
}

#nav-icon1.open span:nth-child(1) {
    top: 12px;
    -webkit-transform: rotate(135deg);
    -moz-transform: rotate(135deg);
    -o-transform: rotate(135deg);
    transform: rotate(135deg);
}

#nav-icon1.open span:nth-child(2) {
    opacity: 0;
    left: -60px;
}

#nav-icon1.open span:nth-child(3) {
    top: 12px;
    -webkit-transform: rotate(-135deg);
    -moz-transform: rotate(-135deg);
    -o-transform: rotate(-135deg);
    transform: rotate(-135deg);
}
}
</style>
