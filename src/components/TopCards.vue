<template>
<div class="top">
<Card class="card" barColor = "hsl(208, 92%, 53%)" platform="facebook" username="nathanf" followersNum="1987" ForS="F O L L O W E R S" upDown="up" diff="12" />
<Card class="card" barColor = "hsl(203, 89%, 53%)" platform="twitter" username="nathanf" followersNum="1044" ForS="F O L L O W E R S" upDown="up" diff="99" />
<Card class="card" barColor = "linear-gradient(90deg, hsl(37,97%,70%) 35%, hsl(329,70%,58%) 100%)" platform="instagram" username="realnathanf" followersNum="11k" ForS="F O L L O W E R S" upDown="up" diff="1099" />
<Card class="card" barColor = "hsl(348, 97%, 39%)" platform="youtube" username="Nathan F." followersNum="8239" ForS="S U B S C R I B E R S" upDown="down" diff="144" />
</div>
</template>

<script>
import Card from "./Card.vue"
export default{
    name:"TopCards",
    components:{
        Card
    }
}
</script>

<style>
.top{
    display: flex;
    justify-content: center;
}
.card{
    margin-left: 25px;
}
.card:hover {
  background-color:rgb(211, 212, 220);
}
</style>