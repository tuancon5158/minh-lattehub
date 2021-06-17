<template>
   <div><a href="#"> <div class="banner">
        <br>
        <div><p>Dress for Every<br>Budget</p></div>
        <div><b>We've got a range of style——featuring on-trend romantic details and midi and<br>maxi lengths——in a range of prices</b></div>
        <br>
        <button>Shop Now</button>
        </div>
    </a>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped lang='css'>
.banner{
    padding: 10%;
    display: flex;
    flex-wrap: wrap;
    max-width: 100%;
    flex-direction: column;
    align-items: center;
    background-image: url('https://minio.lattehub.com/img/2000/2000/resize/60bdc849e0db61849045908f/2021/06/11/lattehub-image-60c2dec02f33d2dfe21c6b17.png');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
   color: ghostwhite;
   filter: brightness(60%);
}
p{
    font-size: 400%;
    font-weight: bold;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
}
a{
     color: black;
    text-decoration: none;
}
button{
    background-color: white;
    color: black;
    border: none;
  text-align: center;
  text-decoration: none;
  font-weight: bold;
  display: inline-block;
  font-size: 120%;
  margin: 1%;
  padding: 0.5%;
  cursor: pointer;
}
</style>