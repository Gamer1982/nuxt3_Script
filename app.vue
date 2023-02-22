<template>
  <div class="container">
    <h1 class="h1">Baby Name Generator</h1>
    <p>choise your options and click the "Find Names" buttom bellow</p>
    <div class="optiions-container">
      <div class="option-container">
        <h4>1) Chose a gender</h4>
        <div class="options-buttons">
          <button>Boy</button>
          <button>Unisex</button>
          <button>Girl</button>
        </div>
      </div>
      <div class="option-container">
        <h4>2) Choose the name's popularity</h4>
        <div class="options-buttons">
          <button>Trendy</button>
          <button>Unique</button>
        </div>
      </div>
      <div class="option-container">
        <h4>3) Choose name's length</h4>
        <div class="options-buttons">
          <button>Long</button>
          <button>All</button>
          <button>Short</button>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  font-family: Arial, Helvetica, sans-serif;
  color: rgb(27, 60, 138);
  max-width: 50rem;
  margin: 0 auto;
  text-align: center;


}

.h1 {
  font-size: 3rem;
}

.optiions-container {
  background-color: rgb(255, 238, 236);

}

.option-container {}

.options-buttons {}
</style>