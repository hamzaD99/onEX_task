<template>
<div class="box">
    <div :style="{'background': barColor}"   class="coloredBar"></div>

    <div class="insideBox">
        <div class="SM">
            <div class="logo">
                <img :src="require(`../assets/icon-${platform}.svg`)" alt="">
            </div>
            <div class="SMUsername"><p class="textInside">@{{username}}</p></div>
        </div>
        <div class="number"><p class="numberInside">{{followersNum}}</p></div>
        <div class="followers"><p class="Followers">{{ForS}}</p></div>
        <div class="bottom">
        <img :src="require(`../assets/icon-${upDown}.svg`)" alt="">
        <p :class="[upDown]">{{diff}} Today</p>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name:"Card",
    props:{
        platform: String,
        username: String,
        followersNum: String,
        ForS: String,
        barColor: Function,
        upDown: String,
        diff: String
    }
}
</script>

<style scoped>
.Followers{
color: hsl(228, 12%, 44%);
  font-size: 10px;
  font-weight: 400;
}
.box{
width: 230px;
height: 200px;
background-color:hsl(227,47%,96%);
border-radius: 5px;
}
.insideBox{
    width: 80%;
    height: 245px;
    display: flex;
    flex-direction: column;
    justify-content: start;
    align-items: center;
    margin-left: 19px;
}
.coloredBar{
width: 100%;
height: 5px;
border-radius: 10px 10px 0px 0px;
}
.number{
    width: 100%;
    height: 50px;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 5px;
}
.followers{
    width: 100%;
    height: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 25px;
}
.SM{
    width: 100%;
    display: flex;
    align-items: center;
    justify-content:center;
    margin-top: 18px;
    margin-bottom: 18px;
}
.bottom{
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
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
.logo{
    margin-right: 7px;
}
.numberInside{
  color: hsl(230, 17%, 14%);
  font-size: 50px;
  font-weight: 700;
}
</style>