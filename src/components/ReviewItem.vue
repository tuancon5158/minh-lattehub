<template>
  <div class="all">
    <div class="title">
      <span class="material-icons" v-for="i in 5" :key="i"> star </span>
      <i class="c">4 hours ago</i>
    </div>
    <br />
    <div class="name"><b>Belinda Asevedo</b></div>
    <br />
    <div class="temp"><b>I absolutely love the cup</b></div>
    <br />
    <div>
      I was very impressed with the quality. The two mugs were gifts for
      Marines. Well worth what I paid. I will do more business with these
    </div>
    <br />
    <div class="svg">
      <div>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          viewBox="0 0 24 24"
          style="color: green"
        >
          <path d="M10 9V5l-7 7 7 7v-4.1c5 0 8.5 1.6 11 5.1-1-5-4-10-11-11z" />
        </svg>
      </div>
      <div>Reply from monolom</div>
      <div>September 4</div>
    </div>
    <div class="button">
      <button>Read more</button>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style scoped lang='css'>
.all {
  text-align: left;
  background-color: #f8f9fa;
  width: 90%;
  margin-bottom: 20%;
}
.name {
  font-size: 90%;
  color: grey;
}
.temp {
  font-size: 90%;
}
.material-icons {
  font-size: 100%;
  color: white;
  border: solid;
  width: 15px;
  background-color: green;
}
.c {
  font-size: 80%;
  padding-left: 2%;
}
.svg {
  border-left: green 0.2pc solid;
}
.svg svg {
  color: green;
  float: left;
}
.button button {
  color: green;
  border: none;
  background-color: #f8f9fa;
  padding: 20%;
  width: 100%;
}
.button button:hover{
  cursor: pointer;
}
@media screen and (max-width: 600px){
.all{
    width: 100%;
}
}
</style>