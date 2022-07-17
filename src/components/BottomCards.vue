<template>
<div class="bottom">
<div class="first">
<BottomCard class="card" title="Page Views" platform="facebook" num="87" per="3" upDown="up" />
<BottomCard class="card" title="Likes" platform="facebook" num="52" per="2" upDown="down" />
<BottomCard class="card" title="Likes" platform="instagram" num="5462" per="2257" upDown="up" />
<BottomCard class="card" title="Profile Views" platform="instagram" num="52k" per="1375" upDown="up" />
</div>
<div class="second">
<BottomCard class="card" title="Retweets" platform="twitter" num="117" per="303" upDown="up" />
<BottomCard class="card" title="Likes" platform="twitter" num="52k" per="553" upDown="up" />
<BottomCard class="card" title="Likes" platform="youtube" num="107" per="19" upDown="down" />
<BottomCard class="card" title="Total Views" platform="youtube" num="1407" per="12" upDown="down" />
</div>
</div>
</template>

<script>
import BottomCard from './BottomCard.vue'
export default{
    name:"BottomCards",
    components:{
        BottomCard
    }
}
</script>

<style scoped>
.botttom{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: start;
}
.first{
    display: flex;
    align-items: center;
    justify-content: center;
}
.second{
    display: flex;
    align-items: center;
    justify-content: center;
}
.card{
    margin: 10px;
}
.card:hover {
  background-color:rgb(211, 212, 220);
}
</style>