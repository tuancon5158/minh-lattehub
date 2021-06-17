<template>
  <div class="card">
    <a href="#"
      ><img
        src="https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/10/latte-image-60c28f597c2ee65f9d1270c0.jpeg"
        style="width: 100%"
      />
      <p>Vintage Floral Print Patchwork Long Sleeve Dress with Pockets</p>
      <p class="price">$19.99</p>
      <button>Add to Cart</button></a
    >
  </div>
</template>
<script>
export default {};
</script>
<style scoped lang='css'>
.card {
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
  max-width: 250px;
  margin: auto;
  margin-top: 0pc;
  padding-top: 0pc;
  text-align: left;
  font-family: arial;
  height: 20pc;
}
.card:hover button {
  visibility: visible;
}
.card a {
  color: black;
  text-decoration: none;
}
.card img {
  height: 15pc;
}
.card p {
  text-align: left;
  padding-left: 1pc;
  padding-right: 1pc;
  overflow: auto;
  overflow-x: hidden;
  font-size: 90%;
}
.price {
  text-align: left;
  color: #0d9ef2;
  font-size: 22px;
}

.card button {
  border: none;
  outline: 0;
  padding: 12px;
  color: white;
  background-color: #0654f3;
  text-align: center;
  cursor: pointer;
  width: 100%;
  font-size: 18px;
  visibility: hidden;
}

.card button:hover {
  opacity: 0.7;
}
</style>