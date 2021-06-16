<template>
    <div class="collection">
        
        <div class="scroll">
        <div class="row">
            <div class="column">
                <BestSellingItem2/>
                
            </div>
            <div class="column">
                <BestSellingItem2/>
                
            </div>
            <div class="column">
                <BestSellingItem2/>
                
            </div>
            <div class="column">
                <BestSellingItem2/>
                
            </div>
            <div class="column">
                <BestSellingItem2/>
                
            </div>
            <div class="column">
                <BestSellingItem2/>
                
            </div>
            <div class="column">
                <BestSellingItem2/>
                
            </div>
            <div class="column">
                <BestSellingItem2/>
                
            </div>
            
        </div>
        
    
    </div>
    </div>
</template>
<script>
import BestSellingItem2 from './BestSellingItem2.vue'
export default {
    components:{
        BestSellingItem2,
    }
}
</script>
<style scoped lang='css'> 
::-webkit-scrollbar {
  height: 0.2pc;
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
.scroll {
  margin-top: 2%;
  width: 60%;
  height: 15pc;
  overflow: auto;
  text-align: center;
  white-space: nowrap;
  overflow-y: hidden;
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