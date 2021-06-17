<template>
  <div class="collection">
    <div class="scroll">
      <div class="row">
        <div class="column">
          <BestSellingItem2 />
        </div>
        <div class="column">
          <BestSellingItem2Copy />
        </div>
        <div class="column">
          <BestSellingItem2Copy2 />
        </div>
        <div class="column">
          <BestSellingItem2Copy3 />
        </div>
        <div class="column">
          <BestSellingItem2Copy4 />
        </div>
        <div class="column">
          <BestSellingItem2Copy5 />
        </div>
        <div class="column">
          <BestSellingItem2 />
        </div>
        <div class="column">
          <BestSellingItem2 />
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import BestSellingItem2 from "./BestSellingItem2.vue";
import BestSellingItem2Copy from "./BestSellingItem2copy.vue";
import BestSellingItem2Copy2 from "./BestSellingItem2copy2.vue";
import BestSellingItem2Copy3 from "./BestSellingItem2copy3.vue";
import BestSellingItem2Copy4 from "./BestSellingItem2copy4.vue";
import BestSellingItem2Copy5 from "./BestSellingItem2copy5.vue";
export default {
  components: {
    BestSellingItem2,
    BestSellingItem2Copy,
    BestSellingItem2Copy2,
    BestSellingItem2Copy3,
    BestSellingItem2Copy4,
    BestSellingItem2Copy5,
  },
};
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
  margin-top: 0%;
  width: 60%;
  height: 15pc;
  overflow: auto;
  text-align: center;
  white-space: nowrap;
  overflow-y: hidden;
  overflow-x: hidden;
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