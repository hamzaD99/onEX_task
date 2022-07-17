<template>
<div class="main">
        <div class="text">
           <div> <p class="Title">Social Media Dashboard</p></div>
            <div><p class="textInside">Total Followers: 23,004</p></div>
            </div>
        <div class="toggle">
            <div><p class="textInside">Dark Mode</p></div>
            <div>
            <label class="switch">
            <input type="checkbox">
            <span class="slider round"></span>
            </label>
            </div>
        </div>
    </div>
</template>

<script>
export default{
    name: "Header",
}
</script>

<style scoped>
.main{
background: rgba(248,249,254,255);
height: 300px;
width: 100%;
display: flex;
justify-content: space-between;
}
.text{
    display: flex;
    flex-direction: column;
    margin-left: 140px;
}
.Title{
    color: hsl(230, 17%, 14%);
  font-size: 30px;
  font-weight: 700;
  margin-bottom: -5px;
}

.toggle{
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 100px;
    margin-bottom: 200px;
    margin-right: 120px;
}

.switch {
  position: relative;
  display: inline-block;
  width: 40px;
  height: 21px;
}

/* Hide default HTML checkbox */
.switch input {
  opacity: 0;
  width: 0;
  height: 0;
}

/* The slider */
.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #ccc;
  -webkit-transition: .4s;
  transition: .4s;
}

.slider:before {
  position: absolute;
  content: "";
  height: 15px;
  width: 15px;
  right: 3px;
  bottom: 3px;
  background-color: white;
  -webkit-transition: .4s;
  transition: .4s;
}

input:checked + .slider {
  background: linear-gradient(90deg, hsl(210,78%,56%) 35%, hsl(146,68%,55%) 100%);
}

input:focus + .slider {
  box-shadow: 0 0 1px linear-gradient(90deg, hsl(210,78%,56%) 35%, hsl(146,68%,55%) 100%);
}

input:checked + .slider:before {
  -webkit-transform: translateX(-19px);
  -ms-transform: translateX(-19px);
  transform: translateX(-19px);
}

/* Rounded sliders */
.slider.round {
  border-radius: 34px;
}

.slider.round:before {
  border-radius: 50%;
}
</style>