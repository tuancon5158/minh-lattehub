<template>
    <div class="collection">
        <BestSellingItem/>
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
.collection{
    display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-around;
  height: 1%
}
@media (max-width: 800px) {
  .collection {
    flex: 100%;
    max-width: 100%;
  }
}

@media (max-width: 600px) {
  .collection {
    flex: 100%;
    max-width: 100%;
  }
}
</style>