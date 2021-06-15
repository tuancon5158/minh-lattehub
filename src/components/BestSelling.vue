<template>
    <div class="collection">
        
        <div class="scroll">
        <div class="row">
            <div class="column">
                <BestSellingItem/>
                
            </div>
            <div class="column">
                <BestSellingItem/>
                
            </div>
            <div class="column">
                <BestSellingItem/>
                
            </div>
            <div class="column">
                <BestSellingItem/>
                
            </div>
            <div class="column">
                <BestSellingItem/>
                
            </div>
            
        </div>
        
    
    </div>
    </div>
</template>
<script>
import BestSellingItem from './BestSellingItem.vue'
export default {
    components:{
        BestSellingItem,
    }
}
</script>
<style scoped lang='css'> 
.scroll {
  margin-top: 2%;
  width: 60%;
  height: 23pc;
  overflow: auto;
  text-align: center;
  white-space: nowrap;
}
.row {
  flex-wrap: wrap;
}
.column {
  display: inline-block;
  padding-left: 2pc;
  flex: 75%;
  max-width: 25%;
  
}
@media (max-width: 800px) {
  .column {
    flex: 75%;
    max-width: 25%;
  }
}

@media (max-width: 600px) {
  .column {
    flex: 100%;
    max-width: 100%;
  }
}
</style>