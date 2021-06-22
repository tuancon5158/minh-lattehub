<template>
  <span class="col">
    <td
      v-for="(collection, key) in collections"
      :collection="collection"
      :key="key"
      style="padding-right: 3%"
      id="web"
    >
      <img :src="collection.img" />
      <p>{{ collection.title }}</p>
    </td>
    <a
      id="mobile"
      v-for="(collection1, k) in collections"
      :collection="collection1"
      :key="k"
    >
      <img :src="collection1.img" />
      <div>{{ collection1.title }}</div>
    </a>
  </span>
</template>
<script>
export default {
  data() {
    return {
      collections: [
        {
          img: "https://minio.lattehub.com/img/1000/1000/resize/60bdc849e0db61849045908f/2021/06/10/lattehub-image-60c1e1eab36aa87e246bcffc.png",
          title: "Accessories",
        },
        {
          img: "https://minio.lattehub.com/img/1000/1000/resize/60bdc849e0db61849045908f/2021/06/10/lattehub-image-60c1d36d79de3a0c7848ae6b.png",
          title: "Dress",
        },
        {
          img: "https://minio.lattehub.com/img/1000/1000/resize/60bdc849e0db61849045908f/2021/06/07/lattehub-image-60bddf51f3292459cb0511d4.gif",
          title: "Bag & Accessories",
        },
        {
          img: "https://minio.lattehub.com/img/1000/1000/resize/60bdc849e0db61849045908f/2021/06/07/lattehub-image-60bddf6b677378a01257ca97.jpeg",
          title: "Footwear & Accessories",
        },
      ],
    };
  },
};
</script>
<style scoped lang='css'>
td:hover{
  cursor: pointer;
}
#mobile {
  display: none;
}
.col {
  display: inline-block;
  text-align: center;
  font-weight: bold;
  font-size: 120%;
  width: 55%;
  padding-left: 25%;
  
}
.col td img {
  width: 100%;
}
@media screen and (max-width: 600px) {
  #mobile {
    display: block;
  }
  #web {
    display: none;
  }
  .col {
    display: block;
    text-align: right;
    padding-left: 5%;
    font-size: 95%;
  }
  .col a {
    width: 100%;
    margin-bottom: 10%;
  }
  .col a img {
    width: 165%;
  }
}
</style>