<template>
    <div class="list">
        <div><h2>Collection list</h2></div>
        <div class="row">
        <div class="collection">
            <div><a href="#"><img src="https://minio.lattehub.com/img/1000/1000/resize/60bdc849e0db61849045908f/2021/06/10/lattehub-image-60c1e1eab36aa87e246bcffc.png"/>Accessories</a></div>
            <div><a href="#"><img src="https://minio.lattehub.com/img/1000/1000/resize/60bdc849e0db61849045908f/2021/06/10/lattehub-image-60c1d36d79de3a0c7848ae6b.png"/>Dress</a></div>
            <div><a href="#"><img src="https://minio.lattehub.com/img/1000/1000/resize/60bdc849e0db61849045908f/2021/06/07/lattehub-image-60bddf51f3292459cb0511d4.gif"/>Bag & Accessories</a></div>
           <div><a href="#"><img src="https://minio.lattehub.com/img/1000/1000/resize/60bdc849e0db61849045908f/2021/06/07/lattehub-image-60bddf6b677378a01257ca97.jpeg"/>Footwear & Accessories</a></div>
        </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped lang='css'>
h2{
    font-weight: bold;
    font-size: 200%;
}
.list{
    padding: 1%;
    display: flex;
    flex-wrap: wrap;
    flex-direction: column;
}
.row{
    display: flex;
  flex-wrap: wrap;
  padding: 0 4px;
}
.collection{
    flex: 25%;
    max-width: 25%;
    padding: 0 4px;
}
.collection img{
   max-width: 100%;
}
a{
    font-size: 100%;
    font-weight: bold;
}
</style>