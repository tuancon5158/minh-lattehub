<template>
  <div>
    <span id="icon" class="web">
      <td>
        <tr class="material-icons"> flight_takeoff</tr><br>
        Standard Shipping Worldwide
      </td>
      <td>
        <tr class="material-icons"> published_with_changes </tr>
        <br>Free Return Worldwide On Orders Over $30
      </td>
      <td>
        <tr class="material-icons"> verified_user </tr>
        <br><b>REMEMBER TO DRINK</b><br>
        100% Safe & Sercure Checkout
      </td>
    </span>
    <span class="mobile">
      <tr>
        <td>
          <tr class="material-icons"> flight_takeoff</tr><br>Standard Shipping
          Worldwide
        </td>
      </tr>
      <tr>
        <td>
          <tr class="material-icons"> published_with_changes </tr><br>Free Return Worldwide On Orders Over $30
        </td>
      </tr>
      <tr>
        <td>
          <tr class="material-icons"> verified_user </tr><br><b>REMEMBER TO DRINK</b><br>100% Safe & Sercure Checkout
        </td>
      </tr>
    </span>
  </div>
</template>
<script>
export default {};
</script>
<style scoped lang='css'>
.material-icons{
  font-size: 350%;
}
.mobile {
  display: none;
}
.web {
  display: inline;
}
#icon {
  margin-left: 24%;
}
td {
  border: 10px solid white;
  width: 22pc;
  height: 5pc;
  text-align: center;
  padding-top: 2%;
  padding-bottom: 2%;
  font-size: 100%;
  color: #3e444b;
  background-color: #ebf0ff;
}
@media screen and (max-width: 1024px){
  #icon {
  margin-left: 0%;
}
}
@media screen and (max-width: 600px) {
  .material-icons{
  font-size: 250%;
}
  .mobile {
    display: inline-block;
  }
  .web {
    display: none;
  }
  td {
    height: 5pc;
    text-align: center;
    padding-top: 5%;
    margin: 0%;
    font-size: 120%;
    color: #3e444b;
    background-color: #ebf0ff;
  }
  tr {
    text-align: center;
    padding-top: 5%;
    font-size: 120%;
    color: #3e444b;
    background-color: #ebf0ff;
  }
}
</style>