<template>
<div> 
  <p ></p>
  <span :style="{color:color,fontsize:10}" v-bind:id="Line1">Добропожаловать</span>
  <p v-bind:id="Line"></p>
  <div>
    <input v-model="login" placeholder="Ваш логин">
    <div>     
    <input v-model="password" placeholder="Ваш пароль">
    </div>
  </div>
  <p v-bind:id="Line"></p>
  <button :style="{color:color}">Войти</button>
  <div>
    <button :style="{color:color}">Зарегистрировать</button>   
  </div>
  
</div>
</template>

<script>
  export default {
    data() {
      return {
        color : '#FF0000',
        height : 100,
      }
    }
  } 
</script>

<style>
#Line {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  line-height: 10%;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#Line1 {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  line-height: 100px;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
