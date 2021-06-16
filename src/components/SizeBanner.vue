<template>
  <div class="size">
    <div class="row">
      <div class="column">
        <div>
           <div> <img
            src="https://minio.lattehub.com/img/200/200/resize/60bdc849e0db61849045908f/2021/06/07/lattehub-image-60bde469347032ca8823a217.png"
          /><h4></h4><i>Standard Shipping Worldwide</i></div>
        </div>
      </div>
      <div class="column">
        <div>
           <div> <img
            src="https://minio.lattehub.com/img/200/200/resize/60bdc849e0db61849045908f/2021/06/07/lattehub-image-60bde47252141727c5ea21cb.jpg"
          /><h4></h4>
          <i>Free Return Worldwide On Orders Over $30</i></div>
        </div>
      </div>
      <div class="column">
        <div>
        
         
          <div><img
            src="https://minio.lattehub.com/img/200/200/resize/60bdc849e0db61849045908f/2021/06/07/lattehub-image-60bde47b09847c6d07ebc13c.png"
          /><h4>REMEMBER TO DRINK</h4> <i>100% Safe & Sercure Checkout</i></div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style scoped lang='css'>
.size {
  padding-top: 1%;
  padding-left: 15%;
  padding-right: 1%;
  padding-bottom: 1%;
  height: 15pc;
}
.row {
  display: flex;
  flex-wrap: wrap;
   margin-bottom: 3pc;
}
.column {
  flex: 75%;
  max-width: 25%;
  height: 7pc;
  margin: 2%;
  margin-bottom: 3pc;
  background-color: lavender;
}
.column img{
float: left;
align-self: center;
margin-left: 1pc;
margin-top: 1pc;
margin-bottom: 1pc;
}
.column div{
    flex-direction: column;
}
.column i{
   width: 100%;
   text-align: center;
}
.column h4 {
  text-align: center;
}
@media (max-width: 800px) {
    .size{
        padding-top: 1%;
  padding-left: 5%;
  padding-right: 5%;
  padding-bottom: 1%;
    }
  .column {
    flex: 100%;
    max-width: 100%;
  }
}

@media (max-width: 600px) {
     .size{
        padding-top: 1%;
  padding-left: 5%;
  padding-right: 5%;
  padding-bottom: 1%;
    }
  .column {
    flex: 100%;
    max-width: 100%;
  }
}
</style>