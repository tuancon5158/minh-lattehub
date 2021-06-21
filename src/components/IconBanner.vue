<template>
  <div>
    <span id="icon" class="web">
      <td>
        <span class="material-icons"> flight_takeoff</span>
        <span>Standard Shipping Worldwide</span>
      </td>
      <td>
        <span class="material-icons"> published_with_changes </span>
        <span>Free Return Worldwide On Orders Over $30</span>
      </td>
      <td>
        <span class="material-icons"> verified_user </span>
        <span><b>REMEMBER TO DRINK</b></span
        ><br />
        <span>100% Safe & Sercure Checkout</span>
      </td>
    </span>
    <span class="mobile">
      <tr>
        <td>
          <span class="material-icons"> flight_takeoff</span>Standard Shipping
          Worldwide
        </td>
      </tr>
      <tr>
        <td>
          <span class="material-icons"> published_with_changes </span>Free Return Worldwide On Orders Over $30
        </td>
      </tr>
      <tr>
        <td>
          <span class="material-icons"> verified_user </span><b>REMEMBER TO DRINK</b><br>100% Safe & Sercure Checkout
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
  font-size: 200%;
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
  padding-top: 5%;
  font-size: 120%;
  color: #3e444b;
  background-color: #ebf0ff;
}
@media screen and (max-width: 600px) {
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