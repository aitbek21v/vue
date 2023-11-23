<template>
  <div id="header">
    <div class="line"></div>
    <div class="container">

      <div class="header">
        <img src="../../assets/logo.svg" alt="Логотип">

        <nav>
          <a href="#">Home</a>
          <a href="#">About Us</a>
          <a href="#">Study Abroad</a>
          <a href="#">Contacts</a>
<!--          <div class="ins">-->
            <input type="search" placeholder="Поиск...">
            <select>
              <option>
                EN
              </option>
              <option>
                RU
              </option>
            </select>
<!--          </div>-->
        </nav>


      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderIndex",
  data(){
    return{
      text:"hello",
    }

  }
}
</script>

<style scoped>
.line {
  width: 1520px;
  height: 9px;background: #FF6A6A;
}
.container {
  width:90%;
  margin: 0 auto;
}
.header {
  padding-top: 20px;
  display: flex;
  align-items: center;
  justify-content:space-between;
}
.header input {
  width: 187px;
  height: 43px;
  flex-shrink: 0;
  border-radius: 10px;
}
.header nav a {
  padding: 0 20px;
  color: black;
  outline: none;
}
.ins input {
  margin: 0 20px;
}
nav input {
  margin: 0 70px;
}
nav select {
  border: none;
}
</style>