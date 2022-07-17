<template>
<div class="Box">
<div class="firstRow">
    <div class="title"><p class="textInside">{{title}}</p></div>
    <div class="logo"><img :src="require(`../assets/icon-${platform}.svg`)" alt=""></div>
</div>
<div class="secondRow">
    <div class="number"><p class="numberInside">{{num}}</p></div>
    <div class="indc">
        <img :src="require(`../assets/icon-${upDown}.svg`)" alt="">
        <p :class="[upDown]">{{per}}%</p>
    </div>
</div>
</div>
</template>


<script>
export default{
    name:"BottomCard",
    props:{
        title: String,
        platform: String,
        num: String,
        per:String,
        upDown: String
    }
}
</script>

<style scoped>
.Box{
    width: 230px;
    height: 125px;
    background-color:hsl(227,47%,96%);
    border-radius: 5px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}
.firstRow{
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-around;
    padding-top: 20px;
}
.secondRow{
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-around;
}
.logo{
    margin-left: 50px;
}
.up{
  color: hsl(162.5, 72%, 41%);
  font-size: 9px;
  font-weight: 700;
  margin-left: 5px;
}
.down{
  color: hsl(357, 69%, 57%);
  font-size: 9px;
  font-weight: 700;
  margin-left: 5px;
}
.numberInside{
  color: hsl(230, 17%, 14%);
  font-size: 30px;
  font-weight: 700;
}
.indc{
    display: flex;
    justify-content: center;
    align-items: center;
    margin-left: 50px;
}
</style>