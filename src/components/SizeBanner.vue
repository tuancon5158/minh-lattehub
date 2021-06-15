<template>
  <div class="size">
    <div class="row">
      <div class="column">
        <div>
           <p> <img
            src="https://minio.lattehub.com/img/200/200/resize/60bdc849e0db61849045908f/2021/06/07/lattehub-image-60bde469347032ca8823a217.png"
          />Standard Shipping Worldwide</p>
        </div>
      </div>
      <div class="column">
        <div>
           <p> <img
            src="https://minio.lattehub.com/img/200/200/resize/60bdc849e0db61849045908f/2021/06/07/lattehub-image-60bde47252141727c5ea21cb.jpg"
          />
          Free Return Worldwide On Orders Over $30</p>
        </div>
      </div>
      <div class="column">
        <div>
        
          <h4>REMEMBER TO DRINK</h4>
          <p><img
            src="https://minio.lattehub.com/img/200/200/resize/60bdc849e0db61849045908f/2021/06/07/lattehub-image-60bde47b09847c6d07ebc13c.png"
          />100% Safe & Sercure Checkout</p>
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
}
.row {
  display: flex;
  flex-wrap: wrap;
}
.column {
  flex: 75%;
  max-width: 25%;
  margin: 2%;
  background-color: lavender;
  align-items: baseline;
}
.column div{
    flex-direction: row;
}
.column p {
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