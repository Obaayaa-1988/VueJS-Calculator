<template>
  <div class="main-bg">
    <h1 class="title"> VUE JS CALCULATOR</h1>

    <div class="calculator">
      <div class="display"> 0.2222 </div>
      <div class="btn"> % </div>
      <div class="btn"> +/- </div>
      <div class="btn"> C </div>
      <div class="btn color"> + </div>
      <div class="btn"> 7 </div>
      <div class="btn"> 8 </div>
      <div class="btn"> 9 </div>
      <div class="btn color"> x </div>
      <div class="btn"> 4 </div> 
      <div class="btn"> 5 </div>
      <div class="btn"> 6 </div>
      <div class="btn color"> - </div>
      <div class="btn"> 1 </div>
      <div class="btn"> 2 </div>
      <div class="btn"> 3 </div>
      <div class="btn color"> / </div>
      <div class="btn zero"> 0 </div>
      <div class="btn"> . </div>
      <div class="btn color"> = </div>   
    </div>

  </div>
</template>

<script>
export default {
  name: "CalculatorApp",

  props: {
    msg: String,
  },
};
</script>

<style scoped>


.main-bg{
  background-color: rgb(98, 62, 182);
  height: 100vh;
  padding: 70px;
  overflow: hidden;
}

.title{
  color: whitesmoke;
  margin-bottom: 3rem;
  font-family: monospace;
}
/* calculator for dividing into grids */ 
.calculator{
  font-size: 40px;
  display: grid; 
  grid-template-columns: repeat(4, 1fr);
  grid-auto-rows: minmax(50px, auto);
  width: 50vh;
  margin: 0 auto
}
/** the display where result of calculator will show, to extend he space grid column to span from from column 1 to 5 1/5*/
.display{
  grid-column: 1/5;
  background-color: aliceblue;
  padding: 30px;
  font-size: 3.5rem;
  border-top-right-radius: 20px;
  border-top-left-radius: 20px;
}
/** zero space span from 1 to 3 1/3*/
.zero{
  grid-column: 1/3;
}

.btn{
  background-color: rgb(94, 95, 175) ;
  /* border: 1px solid #333; */
  padding: 20px;
  color: white;
  cursor: pointer;
}

.color{
  background-color: tomato;
  color: white;
}


</style>
