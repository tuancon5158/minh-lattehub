<template>
  <div class="banner">
    <div class="container">
      <img
        id="img"
        style="width: 100%"
      />
      <div class="centered">
          <p class="title">{{banner.title}}</p>
          <p class="subTitle">{{banner.subTitle}}</p>
          <button v-if="this.banner.has==='1'">SHOP NOW</button>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: ["banner"],
  mounted(){
      document.getElementById("img").setAttribute("src",this.banner.img)
     
  },
};
</script>
<style scoped lang="css">
.banner{
  margin-top: 9%;
}
.container {
  text-align: center;
  color: white;
}
.title{
    font-size: 450%;
    font-weight: bold;
    text-align: center;
    width: 65%;
    margin-bottom: 5%;
    padding-left: 20%;
}
.subTitle{
    margin-top: 0%;
    padding-top: 0%;
    padding-left: 5%;
    font-weight: bold;
    text-align: center;
    margin-bottom: 10%;
}
.centered {
  position: absolute;
  top: 45%;
  left: 50%;
  transform: translate(-50%, -50%);
}
button{
    border: 0;
    width: 15%;
    height: 2pc;
    font-weight: bold;
    background-color: white;
}
button:hover{
  cursor: pointer;
}
@media screen and (max-width: 600px) {
    .centered {
  position: relative;
}
.title{
    font-size: 200%;
    font-weight: bold;
    color: black;
    width: 100%;
    margin-top: 20%;
    margin-bottom: 0%;
    padding-left: 1%;
}
.subTitle{
   visibility: hidden;
}
button{
    margin-top: 0%;
    border: 0;
    width: 70%;
    height: 2pc;
    font-weight: bold;
    color: black;
    background-color: orange;
}
}
</style>