<template>
<div class="header">
<Header />
</div>
<div class="topCards">
<TopCards />
</div>
<div class="today">
  <p class="todayText">Overview - Today</p>
</div>
<BottomCards />
</template>

<script>
import Header from "./components/Header.vue"
import TopCards from "./components/TopCards.vue"
import BottomCards from "./components/BottomCards.vue"
export default {
  name: 'App',
  components: {
    Header,
    TopCards,
    BottomCards
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter&display=swap');
#app {
  font-family: 'Inter';
  background: hsl(0,0%,100%);
}
.textInside{
  color: hsl(228, 12%, 44%);
  font-size: 10px;
  font-weight: 700;
}
.topCards{
  margin-top: -170px;
}
.todayText{
  color: hsl(228, 12%, 44%);
  font-size: 30px;
  font-weight: 700;
}
.today{
  margin-top: 25px;
  margin-left: 140px;
  margin-bottom: -15px;
}
</style>
