<template>
<div id="hero">
  <div class="container">
    <div class="hero">
      <div class="hero-title">
        <h2>Explore the world</h2>
        <h1>Study abroad <br>with our help</h1>
        <p>Study at the world's top universities and <br>expand your horizons. Get the highest <br>quality education and achieve success
          <br>abroad.</p>
      </div>
      <div class="hero--block"/>
      <div>
        <img src="../../assets/bg.svg" alt=""/>
      </div>
      <div class="images">
        <img class="img1" src="../../assets/note.svg" alt=""/>

        <img class="img2" src="../../assets/pass.svg" alt=""/>
        <img class="img3" src="../../assets/black.svg" alt=""/>

        <img class="img4" src="../../assets/katar.svg" alt=""/>

      </div>
    </div>

    <div class="contact">
      <div class="contact">
        <div class=" ">

        </div>
      </div>
    </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeroComponent",
  data() {
    return{
      title:'black'
    }
  }
}
</script>

<style scoped>
.container {
  width:90%;
  margin: 0 auto;
}
#hero {
  padding-top: 130px;
}
.hero {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.hero-title h2 {
  color: rgba(86, 9, 187, 0.80);
  font-size: 24px;
  font-weight: 600;
}
.hero-title h1 {
  color: #000;
  font-size: 64px;
  font-style: normal;
  font-weight: 600;
  line-height: normal;
  letter-spacing: 2.56px;
  text-transform: capitalize;
  margin-top: -4px;
}
.hero-title p {
  color: #606060;
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: 133.336%;
  letter-spacing: 0.72px;
  margin-top: -4px;
}
.hero--block {
  position: relative;
}
.images {
  position: relative;
}
.img1 {
  position: absolute;
  right: 75px;
  bottom: 40px;
}
.img2 {
  position: absolute;
  right: 500px;
  bottom: 85px;
}
.img3 {
  position: absolute;
  /*margin-top: -220px;*/
  right: 410px;
}
.img4 {
  position: absolute;
  right: 150px;
  /*margin-top: -290px;*/
  top: 90px;
}


</style>