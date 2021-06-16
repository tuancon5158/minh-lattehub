<template>
    <div>
        <div class="row"><div><img src="../assets/logo.png" /></div></div>
        <div class="row">
            <div class="column">
                <!-- <div><img src="../assets/logo.png" /><h3 class="contract">Contract Us</h3></div> -->
                <div><h3 class="contract">Contract Us</h3></div>
                <div><p><b>Address:</b>Room 611, Building 3, Hongye Building West Residential Area, Longhua District, Haikou City, Hainan Province</p></div>
                <div><p><b>Email:</b>support@monolom.com</p></div>
            </div>
            <div class="column">
                <div><h3>Our Policies</h3></div>
                <div><a href="#">Privacy policy</a></div>
                <div><a href="#">Terms of services</a></div>
                <div><a href="#">Refund policy</a></div>
                <div><a href="#">Shipping policy</a></div>
                <div><a href="#">DCMA</a></div>
                <div><a href="#">DCMA Report</a></div>
            </div>
            <div class="column">
                <div><h3>Help Center</h3></div>
                <div><a href="#">Contact Us</a></div>
                <div><a href="#">FAQs</a></div>
                <div><a href="#">Cancel/Change Order</a></div>
                <div><a href="#">support@monolom.com</a></div>
                <div><a href="#">Mon - Sat: 9AM - 6PM EST</a></div>
            </div>
        </div>
        <hr style="width:60%;margin-left:20%;color: #ddd">
        <div class="row">
            <div class="column">
                <div><p>© 2021 Monolom.</p></div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped lang="css">
.row {
    padding-left: 20%;
    padding-right: 20%;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
.column {
  flex: 25%;
  max-width: 20%;
}
.column div{
    text-align: left;
}
.column a{
     color: black;
    text-decoration: none;
}
.column a:hover{
    text-decoration: underline;
}
.contract{
   
    visibility: hidden;
   
}
@media (max-width: 800px) {
.contract{
    visibility: visible;
    
}
  .column {
    flex: 100%;
    max-width: 100%;
    overflow: hidden;
  }
}

@media (max-width: 600px) {
    .contract{
    visibility: visible;
}
  .column {
    flex: 100%;
    max-width: 100%;
    overflow: hidden;
  }
}
</style>