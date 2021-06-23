<template>
  <span id='header'>
    <span class="material-icons" id="menu" v-on:click="openNav()"> menu </span>
    <img
      src="https://minio.lattehub.com/img/600/744/resize/60bdc849e0db61849045908f/2021/06/07/lattehub-image-60bdd1cef27e5925329a45c9.png"
      width="150pc" class='logo'
    />
    <a href="#"
      ><button id="search-a">
        <i class="material-icons" id="search"> search </i>What are you searching
        for?
      </button></a
    >
    <i class="material-icons" id="bag"> shopping_bag </i>
    <hr />
    <nav class="nav">
      <ul>
        <li>
          <a href="#"
            >Beauty<span class="material-icons"> arrow_drop_down </span></a
          >
          <ul>
            <li><a href="#">Hair Care</a></li>
            <li><a href="#">Nail Art</a></li>
          </ul>
        </li>
        <li>
          <a href="#"
            >Women's Accessories<span class="material-icons">
              arrow_drop_down
            </span></a
          >
          <ul>
            <li><a href="#">Jewelry & Accessories</a></li>
            <li><a href="#">Footwear & Accessories</a></li>
            <li><a href="#">Leggings</a></li>
            <li><a href="#">Bag & Accessories</a></li>
          </ul>
        </li>
        <li>
          <a href="#"
            >Health Care<span class="material-icons"> arrow_drop_down </span></a
          >
          <ul>
            <li><a href="#">Health</a></li>
          </ul>
        </li>
        <li>
          <a href="#"
            >Life Styles<span class="material-icons"> arrow_drop_down </span></a
          >
          <ul>
            <li><a href="#">Home Improvement</a></li>
            <li><a href="#">Toys</a></li>
          </ul>
        </li>
        <li>
          <a href="#"
            >About Us<span class="material-icons" style="color: white">
              arrow_drop_down
            </span></a
          >
        </li>
        <li id='contract'>
          <a href="#"
            >Contract Us<span class="material-icons" style="color: white">
              arrow_drop_down
            </span></a
          >
        </li>
        <li id='faq'>
          <a href="#"
            >FAQs<span class="material-icons" style="color: white">
              arrow_drop_down
            </span></a
          >
        </li>
      </ul>
    </nav>
    <div id="myNav" class="overlay">
      <a href="javascript:void(0)" class="closebtn" v-on:click="closeNav()"
        >&times;</a
      >
      <hr />
      <div class="overlay-content">
        <li>
          <a href="#" v-on:click="openMiniBeauty()"
            ><p>Beauty</p>
            <span class="material-icons"> add </span></a
          >
          <ul id="beauty">
            <a href="#" class="mini">Hair Care</a>
            <a href="#" class="mini">Nail Art</a>
          </ul>
        </li>
        <li>
          <a href="#" v-on:click="openMiniWomen()"
            ><p>Women's Accessories</p>
            <span class="material-icons"> add </span></a
          >
          <ul id="women">
            <a href="#" class="mini">Jewelry & Accessories</a>
            <a href="#" class="mini">Footwear & Accessories</a>
            <a href="#" class="mini">Leggings</a>
            <a href="#" class="mini">Bag & Accessories</a>
          </ul>
        </li>
        <li>
          <a href="#" v-on:click="openMiniHealth()"
            ><p>Health Care</p>
            <span class="material-icons"> add </span></a
          >
          <ul id="health">
            <a href="#" class="mini">Health</a>
          </ul>
        </li>
        <li>
          <a href="#" v-on:click="openMiniLife()"
            ><p>Life Styles</p>
            <span class="material-icons"> add </span></a
          >
          <ul id="life">
            <a href="#" class="mini">Home Improvement</a>
            <a href="#" class="mini">Toys</a>
          </ul>
        </li>
        <li>
          <a href="#"><p>About Us</p></a>
        </li>
        <li>
          <a href="#"><p>Contract Us</p></a>
        </li>
        <li>
          <a href="#"><p>FAQs</p></a>
        </li>
      </div>
    </div>
  </span>
</template>
<script>
export default {
  methods: {
    openNav() {
      document.getElementById("myNav").style.width = "100%";
      document.getElementById("myNav").style.height= "100pc";
      document.getElementById("myNav").style.backgroundColor="white";
      document.getElementById("myNav").style.position="absolute";
    },

    closeNav() {
      document.getElementById("myNav").style.width = "0%";
      document.getElementById("myNav").style.height="0%";
      document.getElementById("myNav").style.backgroundColor="none";
    },
    openMiniBeauty() {
      document.getElementById("beauty").classList.toggle("show");
      if(document.getElementById("women").classList.contains("show")){
          document.getElementById("women").classList.remove("show");
      }
       if(document.getElementById("health").classList.contains("show")){
          document.getElementById("health").classList.remove("show");
      }
       if(document.getElementById("life").classList.contains("show")){
          document.getElementById("life").classList.remove("show");
      }
    },
    openMiniWomen() {
      document.getElementById("women").classList.toggle("show");
      if(document.getElementById("beauty").classList.contains("show")){
          document.getElementById("beauty").classList.remove("show");
      }
       if(document.getElementById("health").classList.contains("show")){
          document.getElementById("health").classList.remove("show");
      }
       if(document.getElementById("life").classList.contains("show")){
          document.getElementById("life").classList.remove("show");
      }
    },
    openMiniHealth() {
      document.getElementById("health").classList.toggle("show");
      if(document.getElementById("beauty").classList.contains("show")){
          document.getElementById("beauty").classList.remove("show");
      }
       if(document.getElementById("women").classList.contains("show")){
          document.getElementById("women").classList.remove("show");
      }
       if(document.getElementById("life").classList.contains("show")){
          document.getElementById("life").classList.remove("show");
      }
    },
    openMiniLife() {
      document.getElementById("life").classList.toggle("show");
      if(document.getElementById("beauty").classList.contains("show")){
          document.getElementById("beauty").classList.remove("show");
      }
       if(document.getElementById("health").classList.contains("show")){
          document.getElementById("health").classList.remove("show");
      }
       if(document.getElementById("women").classList.contains("show")){
          document.getElementById("women").classList.remove("show");
      }
    },
  },
};
</script>
<style scoped lang='css'>
.material-icons{
  vertical-align: sub;
}
#header{
  margin-top: 0%;
  margin-bottom: 0%;
  padding-top: 0.5%;
}
.logo{
  vertical-align: sub;
}
img:hover{
  cursor: pointer;
}
i:hover{
  cursor: pointer;
}
.mini{
  font-size: 15px !important;
}
.show {
  display: block;
}
.overlay {
  height: 100%;
  width: 0;
  top: 0;
  left: 0;
  background-color: white;
  overflow-x: hidden;
  transition: 0.5s;
}

.overlay-content {
  width: 100%;
  text-align: left;
  margin-top: 0%;
}
.overlay-content li a {
  margin-bottom: 2%;
  width: 100%;
}
.overlay-content li a ul {
  background-color: white;
}
.overlay-content li a p {
  width: 300px;
  margin: auto;
}
.overlay-content li a span {
  display: inline;
  margin-right: 0px;
  text-align: right;
}

.overlay a {
  padding: 8px;
  text-decoration: none;
  font-size: 20px;
  color: #818181;
  display: block;
  transition: 0.3s;
}
.overlay .closebtn {
  font-size: 40px;
  top: 15px;
  right: 35px;
}

#menu {
  display: none;
}
#search-a {
  border: 0.1pc solid;
  border-color: rgb(190, 188, 188);
  display: inline;
  width: 18%;
  text-align: left;
  background-color: white;
  height: 2.5pc;
  color: rgb(190, 188, 188);
  font-size: 100%;
}
#bag {
  margin: 0% 20%;
}
#search {
  padding-right: 10%;
}
img {
  padding-left: 26%;
  padding-right: 5%;
}
.nav {
  text-align: left;
  padding-left: 25%;
  margin-top: 0%;
}
a {
  text-decoration: none;
  text-align: left;
}

hr {
  border-color: rgb(248, 248, 248);
  margin-bottom: 0;
}
ul {
  list-style: none;
  margin: 0;
  padding-left: 0;
}

li {
  display: block;
  float: left;
  padding: 1rem;
  position: relative;
  text-decoration: none;
  transition-duration: 0.5s;
}

li a {
  color: #4f4f4f;
}
li a:hover {
  color: #6f93f5;
  cursor: pointer;
}
li:hover {
  cursor: pointer;
}

ul li ul {
  visibility: hidden;
  opacity: 0;
  min-width: 5rem;
  position: absolute;
  transition: all 0.5s ease;
  margin-top: 1rem;
  left: 0;
  display: none;
}
ul li:hover > ul,
ul li:focus-within > ul,
ul li ul:hover {
  visibility: visible;
  opacity: 1;
  display: block;
  background-color: white;
}

ul li ul li {
  clear: both;
  width: 80%;
}
ul li ul li:hover {
  width: 75%;
  background-color: gainsboro;
}
ul li ul li a:hover {
  color: #4f4f4f;
}
#myNav {
  display: none;
}
@media screen and (max-width: 1024px){
  img{
   padding-left: 0%;
  }
  #search-a {
  border: 0.1pc solid;
  border-color: rgb(190, 188, 188);
  display: inline;
  width: 50%;
  text-align: left;
  background-color: white;
  height: 2.5pc;
  color: rgb(190, 188, 188);
  font-size: 80%;
}
.nav {
  text-align: left;
  padding-left: 4%;
  margin-top: 0%;
  overflow-x: hidden;
}
#bag{
  margin-left: 2%;
}
#contract{
  display: none;
}
#faq{
  display: none;
}
}
@media screen and (max-width: 600px) {
  #search-a {
    border: 0;
    overflow: hidden;
    height: 1.5pc;
    color: black;
    width: 10%;
  }
  #bag {
    margin: 0% 5%;
  }
  img {
    padding-left: 10%;
    padding-right: 5%;
  }
  ul {
    display: none;
  }
  #menu {
    display: inline;
    padding-left: 5%;
  }
  #myNav {
    display: block;
  }
  .material-icons{
  vertical-align: baseline;
}
}
</style>