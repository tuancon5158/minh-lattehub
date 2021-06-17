<template>
  <div class="collection">
    <div class="scroll">
      <div class="row">
        <div class="column">
          <BestSellingItem />
        </div>
        <div class="column">
          <BestSellingItemCopy />
        </div>
        <div class="column">
          <BestSellingItemCopy2 />
        </div>
        <div class="column">
          <BestSellingItemCopy3 />
        </div>
        <div class="column">
          <BestSellingItem />
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import BestSellingItem from "./BestSellingItem.vue";
import BestSellingItemCopy from "./BestSellingItemcopy.vue";
import BestSellingItemCopy2 from "./BestSellingItemcopy2.vue";
import BestSellingItemCopy3 from "./BestSellingItemcopy3.vue";
export default {
  components: {
    BestSellingItem,
    BestSellingItemCopy,
    BestSellingItemCopy2,
    BestSellingItemCopy3,
  },
  data: function () {},
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
  margin-top: 0pc;
  width: 60%;
  height: 23pc;
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