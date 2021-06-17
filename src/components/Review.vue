<template>
  <div class="review">
    <link
      href="https://fonts.googleapis.com/icon?family=Material+Icons"
      rel="stylesheet"
    />
    <div class="title">
      <div>
        <b> Excellent</b>
        <i class="material-icons">start_border</i>
        <i class="material-icons">start_border</i>
        <i class="material-icons">start_border</i>
        <i class="material-icons">start_border</i>
        <i class="material-icons">start_border</i>
      </div>
    </div>
    <div>
      <br />
      Rated<b> 4.3</b> / 5 based on <b>10,991 reviews</b> on<b> Trustpiot</b>
    </div>
    <div class="scroll">
        <div class="row">
            <div class="column">
                <ReviewItem/>
                <ReviewItem/>
                <ReviewItem/>
                
            </div>
            <div class="column">
                <ReviewItem/>
                <ReviewItem/>
                <ReviewItem/>
               
            </div>
            <div class="column">
                <ReviewItem/>
                <ReviewItem/>
                <ReviewItem/>
                
            </div>
             <div class="column">
                <ReviewItem/>
                <ReviewItem/>
                <ReviewItem/>
                
            </div>
        </div>
    
    </div>
  </div>
</template>
<script>
import ReviewItem from './ReviewItem.vue'
export default {
    components:{
ReviewItem
    }
    
};
</script>
<style scoped lang='css'>

.row {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  margin: 0.1%;
}
.column {
  flex: 75%;
  max-width: 25%;
  
}
.material-icons {
  font-size: 75%;
  color: white;
  border: solid;
  width: 15px;
  background-color: green;
}
.title {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  padding-top: 1%;
  padding-left: 45%;
  padding-right: 1%;
  padding-bottom: 1%;
}
.title div {
  text-align: center;
  font-size: 150%;
}
.scroll {
  margin-top: 2%;
  width: 50%;
  height: 20pc;
  overflow-y: visible;
  overflow-x: hidden;
  text-align: center;
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
.review{
  margin-top: 1pc;
  margin-bottom: 5pc;
}
@media (max-width: 800px) {
  .title {
    padding-top: 1%;
    padding-left: 35%;
    padding-bottom: 1pc;
  }
 .column{
    flex: 100%;
    max-width: 100%;
 }
 .review{
  margin-top: 20pc;
  margin-bottom: 15pc;
}
}



@media (max-width: 600px) {
  .title {
    padding-top: 1%;
    padding-left: 35%;
    padding-bottom: 1pc;
  }
  .column{
    flex: 100%;
    max-width: 100%;
 }
 .review{
  margin-top: 20pc;
  margin-bottom: 15pc;
}
}
</style>