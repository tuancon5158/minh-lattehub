<template>
  <div class="review">
    <div class="title">
      <div>
        <b> Excellent</b>
        <span class="material-icons" v-for="i in 5" :key="i"> star </span>
      </div>
      
    </div>
    <div class="subTitle">Rated<b> 4.3</b> / 5 based on <b>10,991 reviews</b> on<b> Trustpiot</b></div>
    <div class="scroll">
      <div class="row">
        <div class="column" v-for="j in 4" :key="j">
          <ReviewItem v-for="i in 3" :key="i"/>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import ReviewItem from "./ReviewItem.vue";
export default {
  components: {
    ReviewItem,
  },
};
</script>
<style scoped lang='css'>
.row {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  margin: 0.1%;
}
.column {
  flex: 75%;
  max-width: 25%;
}
.material-icons {
  font-size: 100%;
  color: white;
  border: solid;
  width: 22px;
  background-color: green;
}
.title {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  padding-top: 1%;
  padding-left: 45%;
  padding-right: 1%;
  padding-bottom: 1%;
}
.subTitle{
    padding-left: 43%;
}
.title div {
  text-align: center;
  font-size: 150%;
}
.scroll {
  margin-top: 2%;
  width: 58%;
  height: 35pc;
  margin-left: 25%;
  overflow-y: visible;
  overflow-x: hidden;
  text-align: center;
}
::-webkit-scrollbar {
  width: 0.2pc;
}
::-webkit-scrollbar-track {
  background: grey;
}

::-webkit-scrollbar-thumb {
  background: #888;
}
::-webkit-scrollbar-thumb:hover {
  background: #555;
}
.review {
  margin-top: 1pc;
  margin-bottom: 10pc;
}
@media screen and (max-width: 1024px){
  .title {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  padding-top: 1%;
  padding-left: 35%;
  padding-right: 1%;
  padding-bottom: 1%;
}
.subTitle{
    padding-left: 25%;
}
.scroll {
  margin-top: 2%;
  width: 100%;
  height: 35pc;
  margin-left: 2%;
  overflow-y: visible;
  overflow-x: hidden;
  text-align: center;
}
}
@media screen and (max-width: 600px) {
    .review{
        margin-top: 0%;
        padding-top: 0%;
    }
    .scroll{
        margin: 0%;
        width: 100%;
        padding: 0%;
    }
  .title {
    margin: 0%;
    padding-top: 0%;
    padding-left: 20%;
    padding-bottom: 0%;
  }
  .subTitle{
      padding-left: 3%
  }
  .column {
    flex: 100%;
    max-width: 100%;
  }
  .review {
    margin-top: 20pc;
    margin-bottom: 15pc;
  }
}
</style>