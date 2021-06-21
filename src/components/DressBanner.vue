<template>
  <div class="col">
    <div class="row">
      <div class="column">
        <div>
         <figure> <img
            src="https://minio.lattehub.com/img/600/600/resize/60bdc849e0db61849045908f/2021/06/07/lattehub-image-60bde2c2b4a0ca0f85ca7317.png"
          /></figure>
        </div>
      </div>
      <div class="column">
        <div class="title">
          <h1>Getting dressed up?</h1>
          <p>
            Shop by style, body type, occasion and more, and find the perfect
            dress! Whether you’re heading to work or to a wedding, there’s a
            frock that fits. Browse the selection of classic or contemporary
            dresses in for amazing styles.
          </p>
          <br /><button><a href="#">VIEW MORE</a></button>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="column">
        <div class="title">
          <h1>Dresses for women.</h1>
          <p>
            Enjoy quality, fashionable women's clothing from Modefeme. Whether
            you're just looking to refresh your wardrobe, add some special
            pieces or overhaul it completely, Modefeme has the women's clothing
            that will add something special to any wardrobe. Getting ready for a
            formal occasion?
          </p>
          <br />
          <button><a href="#">VIEW MORE</a></button>
        </div>
      </div>
      <div class="column">
        <div>
         <figure> <img
            src="https://minio.lattehub.com/img/600/600/resize/60bdc849e0db61849045908f/2021/06/07/lattehub-image-60bde2f3f9cc5b56291e48e8.png"
          /></figure>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style scoped lang='css'>
/* .col {
  display: flex;
  flex-wrap: wrap;
  margin: 1%;
} */
.row {
    margin-top: 2%;
  display: flex;
  flex-wrap: wrap;
   align-items: center;
  justify-items: center;
  overflow: auto;
  overflow-y: hidden;
  overflow-x: hidden;
}
.column {
  flex: 100%;
  max-width: 50%;
}
.column img {
  
  width: 100%;
  
}
a{
  color: white;
  text-decoration: none;
}
.column p {
  text-align: left;
  font-size: 100%;
}
.column h1 {
    font-size: 200%;
  text-align: left;
}
.title{
    margin: 10%;
    text-align: left;
}
.column figure img{
    transform: scale(1);
    transition: 1.5s all ease-in-out;
}
.column figure:hover img{
    transform: scale(1.2);
}
.column button {
  background-color: #0654f3;
  color: white;
  width: 25%;
  padding: 2%;
  border: none;
  font-size: 100%;
  font-weight: bold;
}
@media screen and (max-width: 600px) {
  .column {
    flex: 100%;
    max-width: 100%;
  }
  .column h1 {
    font-size: 200%;
  text-align: center;
}
.title{
    margin: 0%;
    text-align: center;
}
.column button {
  background-color: #0654f3;
  color: white;
  width: 50%;
  height: 45px;
  padding: 2%;
  border: none;
  font-size: 100%;
  font-weight: bold;
}
.column img {
  
  width: 100%;
  margin: 0%;
  padding: 0%;
}
.column figure{
  width: 100%;
  margin: 0%;
  padding: 0%;
}
}
</style>