<script>

export default{
data:()=>({
  contador:10,

}),
methods:{
reset(){
 this.contador=10;
},
},
};



</script>

<template>
<div class="container">
  <img src="./assets/logo.svg" alt="Logo Vue" width="80" height="80" />
  <h1>Hola Mundo Desde Vue.js 3</h1>
  <hr />
  <h2>Contador: {{contador}}</h2>
  <button @click="contador++">+1</button>
  <button @click="contador--">-1</button>
  <button @click="reset()">Reset</button>

</div>
</template>
<style scoped>

.container{
 text-align: center;

}
h1{
 font-weight: bolder;
 color: rgb(73, 72, 72);
}
h2{
  font-size: 2.5rem;
}
button{
  cursor: pointer;
  font-size: 1.5rem;
  margin:  0px 5px;
}

</style>

