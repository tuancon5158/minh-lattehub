<template>
  <span class="col">
    <td v-for="(item,key) in items" :item="item" :key="key" id="web" style="padding-right: 2pc">
        <img :src="item.img"/>
        <p class="title">{{item.title}}</p>
        <p class="price">{{item.price}}</p>
        <button>ADD TO CART</button>
    </td>
    
  </span>
</template>
<script>
export default {
  props:['items'],
};
</script>
<style scoped lang='css'>
.col {
  display: inline-block;
  text-align: center;
  font-weight: bold;
  font-size: 120%;
  width: 65%;
  margin-left: 25%;
  margin-top: 0%;
  padding-top: 0%;
}
p{
    overflow: hidden;
}
.col td{
   width: 240px; 
   position: relative;
}
.col td:hover{
  cursor: pointer;
}
.col td:hover button{
    visibility: visible;
}
.col td img {
  width: 100%;
  height: 250px;
  margin-right: 10px;
}
.title{
    font-weight: normal !important;
    height: 50px;
    text-align: left;
    padding-left: 10px;
    font-size: 14px;
}
.price{
    color: lightskyblue !important;
    font-weight: normal !important;
    text-align: left;
    padding-left: 10px;
}
button{
  visibility: hidden;
  border: none;
  background-color: #0654f3 !important;
  color: white !important;
  font-size: 100% !important;
  font-weight: bold;
  width: 90%;
  height: 2.5pc;
  margin-top: 1%;
  margin-bottom: 3%;
}
button:hover{
  cursor: pointer;
}
@media screen and (max-width: 1024px){
.col {
  display: inline-block;
  text-align: center;
  font-weight: bold;
  font-size: 120%;
  width: 100%;
  margin-left: 2%;
  margin-top: 0%;
  padding-top: 0%;
}
.col td img {
  width: 100%;
  height: 12pc;
  margin-right: 10px;
}
}
@media screen and (max-width: 800px){
.col {
  display: inline-block;
  text-align: center;
  font-weight: bold;
  font-size: 120%;
  width: 100%;
  margin-left: 2%;
  margin-top: 0%;
  padding-top: 0%;
}
.col td img {
  width: 100%;
  height: 10pc;
  margin-right: 10px;
}
}
@media screen and (max-width: 600px) {
    .col {
  display: flexbox;
  text-align: center;
  font-weight: bold;
  font-size: 120%;
  width: 100%;
  margin: 10px;
  overflow: hidden;
}
.col td{
   width: 180px; 
   height: 100px;
   display: flexbox;
}
.col td img {
  width: 150px;
  height: 150px;
  margin-right: 10px;
}
button{
    visibility: visible;
}
}
</style>