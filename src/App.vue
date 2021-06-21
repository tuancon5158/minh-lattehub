<template>
  <div id="app">
    <Header id="header" />
    <br>
    <Banner v-bind:banner="banners[0]"/>
    <br>
    <b id="colection">Collection list</b>
    <Collection/>
    <br>
    <div class="barHome"><b class="titleHome">Best Selling</b><button class="buttonHome">VIEW MORE</button> </div>
    <BestSelling v-bind:items="itemsBestSelling"/>
    <br>
    <img src="https://minio.lattehub.com/img/2000/2000/resize/60bdc849e0db61849045908f/2021/06/11/lattehub-image-60c2dec02f33d2dfe21c6b17.png" height="15%" width="100%">
    <br>
    <DressBanner/>
    <br>
    <div class="barHome"><b class="titleHome">Look we love</b><button class="buttonHome">VIEW MORE</button> </div>
    <BestSelling v-bind:items="itemsLove"/>
    <b id="seller">Store best sellers</b>
    <ItemRecommendation v-bind:items="itemsBestSeller"/>
    <b id="recomendation">Recently viewed & featured recommendations</b>
    <ItemRecommendation v-bind:items="itemsRecommendation"/>
    <br>
    <IconBanner/>
    <Review id="review"/>
    <br>
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Banner from "./components/Banner.vue";
import Collection from "./components/Collection.vue"
import BestSelling from "./components/BestSelling.vue"
import DressBanner from "./components/DressBanner.vue"
import ItemRecommendation from "./components/ItemRecommendation.vue"
import IconBanner from "./components/IconBanner.vue"
import Review from "./components/Review.vue"
export default {
  name: "App",
  components: {
    Header,
    Footer,
    Banner,
    Collection,
    BestSelling,
    DressBanner,
    ItemRecommendation,
    IconBanner,
    Review
  },
  data() {
    return {
      banners: [
        {
          title: "SIXTH COLLECTION",
          subTitle: "Be Sexier - Be deeper in relationship",
          img: "https://minio.lattehub.com/img/2000/2000/resize/60bdc849e0db61849045908f/2021/06/09/lattehub-image-60c09bdc5793c9149caa93e4.jpeg",
          has: "1"
        },
        {
          title: "",
          subTitle: "",
          img: "https://minio.lattehub.com/img/2000/2000/resize/60bdc849e0db61849045908f/2021/06/11/lattehub-image-60c2dec02f33d2dfe21c6b17.png",
          has: "0"
        },
      ],
      itemsBestSelling: [
      {
        title: "Plaid Long Sleeve Loose Crew Neck Plus Size Vintage Dress",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/10/latte-image-60c28f56ac749aaeacb476f1.jpeg",
        price:"$28.97"
      },
       {
        title: "Vintage Women Solid 3/4 Sleeve Loose Maxi Dress For Women",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/10/latte-image-60c28f567c2ee6ea1212709c.jpeg",
        price:"$28.97"
      },
       {
        title: "Vintage Floral Print Patchwork Long Sleeve Dress with Pockets",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/10/latte-image-60c28f597c2ee65f9d1270c0.jpeg",
        price:"$28.97"
      },
       {
        title: "Women Floral Wrap Dress Off Shoulder Tie Up Front Ruffle Mini Dress Summer Office Lady Slash Neck Printed Pencil Dress",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/10/latte-image-60c28f8c7c2ee62b24127279.jpeg",
        price:"$28.97"
      },
    ],
    itemsLove: [
      {
        title: "White Sexy Dress Women Spaghetti Strap Dresses Female High Waist Sheath Club Dress Short Summer 2021 Mini Sleeveless Vestidos",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/10/latte-image-60c28fed7c2ee6dc4e1274f7.jpeg",
        price:"$28.97"
      },
       {
        title: "2021 New Summer Women Bikini Cover Up Floral Lace Hollow Crochet Swimsuit Cover-Ups Bathing Suit Beachwear Tunic Beach Dress Hot",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/10/latte-image-60c28ff17c2ee609ea127540.jpeg",
        price:"$28.97"
      },
       {
        title: "Hirigin Ribbed Mini Dress Women Off Shoulder Sexy Party O Neck Drawstring Knit Club Tank Bodycon Short Women's Summer Dresses",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/10/latte-image-60c28ff07c2ee61f6212753d.jpeg",
        price:"$28.97"
      },
       {
        title: "Casual Boho Beach Dresses  Womens O-Neck Party Summer Dress Short Sleeve Loose Mini Dress",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/10/latte-image-60c28ff3ac749a79acb47afc.jpeg",
        price:"$28.97"
      },
    ],
    itemsBestSeller: [
      {
        title: "Car Auto Eyeglasses Organizer",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/17/latte-image-60cb2c8f49951ea491302b61.gif",
        price:"$28.97"
      },
      {
        title: "36PCS Reusable Chalk Label Set",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/17/latte-image-60cb2c869b74ec3f3e4f2506.jpg",
        price:"$28.97"
      },
      {
        title: "Secret Fringe Braid Bang for Women",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/17/latte-image-60cb2c8549951e1154302aa8.jpeg",
        price:"$28.97"
      },
      {
        title: "The Cool \"Ducky\" Light Horn",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/17/latte-image-60cb2c8449951e0a20302aa1.jpg",
        price:"$28.97"
      },
      {
        title: "Highlight Fluffy Side Hair Extension",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/17/latte-image-60cb2c889b74ec504f4f28b5.jpg",
        price:"$28.97"
      },
      {
        title: "Seamless Hair Toppers With Bangs For Thin Hair",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/17/latte-image-60cb2c8f9b74eccd7f4f29a8.gif",
        price:"$28.97"
      },
    ],
    itemsRecommendation: [
      {
        title: "Plaid Long Sleeve Loose Crew Neck Plus Size Vintage Dress",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/10/latte-image-60c28f56ac749aaeacb476f1.jpeg",
        price:"$28.97"
      },
      {
        title: "Electric Garlic Masher Machine",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/17/latte-image-60cb31a59b74ecbb524f4f18.jpg",
        price:"$28.97"
      },
      {
        title: "Clip-In Natural Seamless Hair",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/17/latte-image-60cb2ca59b74ec4b934f2c1f.jpg",
        price:"$28.97"
      },
      {
        title: "Women's Pearls Headbands White Faux Pearl Rhinestones Hairbands",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/17/latte-image-60cb2cae9b74ec9fa04f2cc9.jpg",
        price:"$28.97"
      },
      {
        title: "Seamless Volumizing Hair Crown For Hair Thinning & Bald Spot",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/17/latte-image-60cb2ca59b74ec1a1d4f2c26.jpg",
        price:"$28.97"
      },
      {
        title: "Seamless Voluminous Long Wavy Headband Human Hair Wig for Women",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/17/latte-image-60cb2c9d9b74ec6a6c4f2b79.gif",
        price:"$28.97"
      },
    ],
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 0%;
  overflow-x: hidden; 
}
#header {
  position: fixed;
  width: 100%;
  background-color: white;
  opacity: 95%;
  margin-top:0% ;
  margin-bottom: 1%;
  z-index: 100;
  padding-top: 0%;
}
#colection{
  text-align: center;
  padding-left: 45%;
  font-size: 200%;
  font-weight: bold;
}
#seller{
  text-align: center;
  padding-left: 45%;
  font-size: 200%;
  font-weight: bold;
}
#recomendation{
text-align: center;
  padding-left: 37%;
  font-size: 200%;
  font-weight: bold;
}
.titleHome{
  padding-left: 25%;
  font-size: 180%;
}
.barHome{
  padding-top: 1%;
  padding-bottom: 0%;
  margin-bottom: 0%;
}
.buttonHome{
  margin-left: 36%;
  border: none;
  background-color: #0654f3 !important;
  color: white !important;
  font-size: 160% !important;
  font-weight: bold;
  width: 10%;
  height: 3pc;
}
img{
  padding: 0;
  margin: 0;
}
@media screen and (max-width: 600px) {
  #app div{
  margin-bottom: 2%;
}
  #app{
    padding: 0;
    margin: 0;
  }
  #colection{
  font-weight: bold;
  text-align: center;
  padding-left: 28%;
  font-size: 180%;
}
#seller{
  font-weight: bold;
  text-align: center;
  padding-left: 23%;
  font-size: 180%;
}
#recomendation{
  text-align: center;
  padding-left: 0%;
  font-size: 180%;
  font-weight: bold;
}
.buttonHome{
  margin-left: 25%;
  border: none;
  background-color: #0654f3 !important;
  color: white !important;
  font-size: 100% !important;
  font-weight: bold;
  width: 50%;
  height: 2.5pc;
  margin-top: 1%;
}
.titleHome{
  padding-left: 30%;
  font-size: 180%;
}
#review{
  margin-top: 0%;
  padding-top: 0%;
}
}
</style>
