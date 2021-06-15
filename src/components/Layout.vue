<template>
  <div>
    <center>
    <div class="header">
      <div class="row-header">
        <a href="#" style="flex-grow: 0.05"><img src="../assets/logo.png" /></a>
        <input type="text" placeholder="Search.." style="flex-grow: 0.2 " />
        <a href="#" style="flex-grow: 0.7"><img src="../assets/icon-bill.png" /></a>
      </div>
      <hr style="width:100%;text-align:left;margin-left:0;color: #ddd">
      <div class="navbar">
        <div class="dropdown">
          <button class="dropbtn">
            Beauty ▼
            <i class="fa fa-caret-down"></i>
          </button>
          <div class="dropdown-content">
            <a href="#">Hair Care</a>
            <a href="#">Nail Art</a>
          </div>
        </div>
        <div class="dropdown">
          <button class="dropbtn">
            Women's Accessories ▼
            <i class="fa fa-caret-down"></i>
          </button>
          <div class="dropdown-content">
            <a href="#"> Jewelry & Accessories </a>
            <a href="#"> Footwear & Accessories </a>
            <a href="#"> Leggings </a>
            <a href="#"> Bag & Accessories </a>
          </div>
        </div>
        <div class="dropdown">
          <button class="dropbtn">
            Health Care ▼
            <i class="fa fa-caret-down"></i>
          </button>
          <div class="dropdown-content">
            <a href="#"> Health</a>
          </div>
        </div>
        <div class="dropdown">
          <button class="dropbtn">
            Life Styles ▼
            <i class="fa fa-caret-down"></i>
          </button>
          <div class="dropdown-content">
            <a href="#">Home Improvement</a>
            <a href="#">Toys</a>
          </div>
        </div>
          <div class="dropdown">
          <button class="dropbtn">
            About Us
            <i class="fa fa-caret-down"></i>
          </button>
        </div>
         <div class="dropdown">
          <button class="dropbtn">
            Contract Us
            <i class="fa fa-caret-down"></i>
          </button>
        </div>
       <div class="dropdown">
          <button class="dropbtn">
            FAQs
            <i class="fa fa-caret-down"></i>
          </button>
        </div>
      </div>
    </div>
    <div class="body">
        <Banner/>
        <CollectionList/>
        <div class="title"><h2 >Best Selling</h2><button>VIEW MORE</button> </div>
        <BestSelling/>
        <Banner2/>
        <DressBanner/>
        <!-- <div class="title"><h2 >Look we love</h2><button>VIEW MORE</button> </div>
        <BestSelling/> -->
        <!-- <div class="title"><h2>Store best sellers</h2></div>
        <BestSelling/> -->
        <div class="title"><h2>Recently viewed & featured recommendations</h2></div>
        <BestSelling/>
        <SizeBanner/>
        <Review/>
    </div>
    <div class="footer">
        <Footer/>
    </div>
    </center>
  </div>
</template>
<script>
import Banner from './Banner.vue'
import Banner2 from './Banner2.vue'
import CollectionList from './CollectionList.vue'
import BestSelling from './BestSelling.vue'
import DressBanner from './DressBanner.vue'
import SizeBanner from './SizeBanner.vue'
import Footer from './Footer.vue'
import Review from './Review.vue'
export default {
    components: {
    Banner,
    Banner2,
    CollectionList,
    BestSelling,
    DressBanner,
    SizeBanner,
    Footer,
    Review
  }
};

</script>
<style scoped lang='css'>
.row-header {
  padding-left: 25%;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-around;
}
.navbar {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-around;
  overflow: hidden;
  
  background-color: white;
}

.navbar a {
  font-size: 16px;
  color: grey;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

.dropdown {
  float: left;
  overflow: hidden;
}

.dropdown .dropbtn {
  font-size: 16px;
  border: none;
  outline: none;
  color: dimgray;
  padding: 14px 16px;
  background-color: inherit;
  font-family: inherit;
  margin: 0;
}

.navbar a:hover,
.dropdown:hover .dropbtn {
  color: lightskyblue;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
  z-index: 1;
}

.dropdown-content a {
  float: none;
  color: dimgray;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
  text-align: left;
}

.dropdown-content a:hover {
  background-color: #ddd;
  color: dimgray;
}

.dropdown:hover .dropdown-content {
  display: block;
}
.title{
  display: flex;
  justify-content: space-around;
}
button{
  background-color: #0654f3;
  color: white;
  width: 12%;
  border: none;
}
@media (max-width: 800px) {
  .navbar{
    opacity: 0;
    visibility: hidden;
    display: none;
  }
}

@media (max-width: 600px) {
   .navbar{
     opacity: 0;
    visibility: hidden;
    display: none;
  }
}
</style>