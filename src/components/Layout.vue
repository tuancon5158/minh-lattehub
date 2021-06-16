<template>
  <div>
    <center>
    <div class="header">
      <div class="row-header">
        <a href="#" style="flex-grow: 0.05"><img src="../assets/logo.png" /></a>
       <div><input class="search" type="text" placeholder="What are you searching for?" style="flex-grow: 0.2 ">
       <button>Cancel</button></div>
        <a href="#" style="flex-grow: 0.7"><img src="../assets/icon-bill.png" /></a>
      </div>
      <hr style="width:100%;text-align:left;margin-left:0;color: #ddd">
      <div class="navbar">
        <div class="dropdown">
          <button class="dropbtn">
            Beauty 
            <i class="fa-caret-down"></i>
          </button>
          <div class="dropdown-content">
            <a href="#">Hair Care</a>
            <a href="#">Nail Art</a>
          </div>
        </div>
        <div class="dropdown">
          <button class="dropbtn">
            Women's Accessories 
            <i class="fa-caret-down"></i>
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
            Health Care 
            <i class="fa-caret-down"></i>
          </button>
          <div class="dropdown-content">
            <a href="#"> Health</a>
          </div>
        </div>
        <div class="dropdown">
          <button class="dropbtn">
            Life Styles 
            <i class="fa-caret-down"></i>
          </button>
          <div class="dropdown-content">
            <a href="#">Home Improvement</a>
            <a href="#">Toys</a>
          </div>
        </div>
          <div class="dropdown">
          <button >
            About Us
            
          </button>
        </div>
         <div class="dropdown">
          <button >
            Contract Us
            
          </button>
        </div>
       <div class="dropdown">
          <button >
            FAQs
            
          </button>
        </div>
      </div>
    </div>
    <div class="body">
        <Banner/>
        <CollectionList/>
        <br>
        <br>
        <div class="title"><h2 >Best Selling</h2><button>VIEW MORE</button> </div>
        <BestSelling/>
        <Banner2/>
        <DressBanner/>
        <br>
        <br>
        <div class="title"><h2 >Look we love</h2><button>VIEW MORE</button> </div>
        <BestSelling/>
        <div class="title"><h2>Store best sellers</h2></div>
        <BestSelling2/>
        <div class="title"><h2>Recently viewed & featured recommendations</h2></div>
        <BestSelling2/>
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
import BestSelling2 from './BestSelling2.vue'
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
    BestSelling2,
    DressBanner,
    SizeBanner,
    Footer,
    Review,
  }
};

</script>
<style scoped lang='css'>
.search{
  width: 20pc;
  box-sizing: border-box;
  border: 1px solid #ccc;
  font-size: 0.9pc;
  background-color: white;
  background-image: url('../assets/search-icon.png');
  background-position: 10px 10px; 
  background-repeat: no-repeat;
  padding: 12px 20px 12px 40px;
  -webkit-transition: width 0.4s ease-in-out;
  transition: width 0.4s ease-in-out;
  margin-left: 5pc;
}
.header{
  background-color: white;
  width: 100%;
  top: 0;
  position: fixed;
    z-index: 999;
  transition: 0.2s;
  opacity: 95%;
  
}
::-webkit-scrollbar {
  width: 0.2pc;
}


::-webkit-scrollbar-track {
  background: grey; 
}
 

::-webkit-scrollbar-thumb {
  background: #888; 
}


::-webkit-scrollbar-thumb:hover {
  background: #555; 
}
.row-header {
  margin-top: 1pc;
  padding-left: 25%;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}
.row-header button{
  visibility: hidden;
}
.navbar {
  padding-left:26%;
  padding-right: 25%;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  overflow: hidden;
  border-bottom: none;
  background-color: white;
  justify-content: space-between;
}

.navbar a {
  font-size: 16px;
  margin-right: 5%;
  color: grey;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

.dropdown {
  float: left;
  overflow: hidden;
  color: dimgray;
}
.dropdown button{
 font-size: 16px;
  border: none;
  outline: none;
  color: dimgray;
  padding: 14px 16px;
  background-color: inherit;
  font-family: inherit;
  margin: 0;
}
.dropdown .dropbtn {
 
  background: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100' fill='%238C98F2'><polygon points='0,0 100,0 50,50'/></svg>") no-repeat;
  background-size: 12px;
  background-position: right;
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
  font-weight: bold;
}
.title button{
  background-color: #0654f3;
  color: white;
  width: 12%;
  height: 4pc;
  border: none;
  font-size: 120%;
  font-weight: bold;
}
@media (max-width: 800px) {
  .navbar{
    opacity: 0;
    visibility: hidden;
    display: none;
  }
  .search{
    justify-self: left;
    width: 1pc;
  }
}

@media (max-width: 600px) {
   .navbar{
     opacity: 0;
    visibility: hidden;
    display: none;
  }
  .search{
    justify-self: left;
    width: 1pc;
  }
}
</style>