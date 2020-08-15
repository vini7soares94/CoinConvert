<template>

  <div id="app">
    <header>
      <img class="top" src="./assets/money.png" alt="Imagem Moeda">
    <h1 class="title-center">Coin Convert</h1>
    </header>

  <div class="line">
    <Conversor moeda-a="BTC" moeda-b="BRL"/>
    <Conversor moeda-a="USD" moeda-b="BRL"/>
    <Conversor moeda-a="EUR" moeda-b="BRL"/>
  </div>
  </div>
</template>

<script>
import Conversor from "./components/Conversor.vue";
export default {
    name: 'App',
    components: { Conversor } 
}
</script>

<style>
body{
  background: #333333;
}
#app {
  margin: auto;
  max-width: 900px;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  margin-top: 60px;
}
footer
{
  background: #000000;
  text-align: center;
  width: 100%;
  margin-top: 20px;
  height: 40px;
  justify-content: center;
  padding: 50px 0;
}
footer a
{
  text-decoration: none;
  color: white;
  font-size: 20px;
}
footer p
{
  color:gray;
  font-size:20px;
  font-weight: bolder;
}
.top {
  width: 60px;
  height: 60px;
  margin-bottom: 30px;
  margin-left: 0;
  margin-right: 0;
  margin: auto;
  display: flex;
}
.line{
  color: gray;
  justify-content: space-around;
  margin-top: 40px;
  display: flex;
  align-items: center;
  justify-items: auto;
}
.title-center{
  text-align: center;
  color: gray;}
</style>
