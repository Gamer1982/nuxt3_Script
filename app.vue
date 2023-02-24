<template>
  <div class="container">
    <h1 class="h1">Baby Name Generator</h1>
    <p>choise your options and click the "Find Names" buttom bellow</p>
    <div class="optiions-container">
      <div class="option-container">
        <h4>1) Chose a gender</h4>
        <div class="options-buttons">
          <button @click="options.gender = 'Boy'" class="btn"
            :class="options.gender === 'Boy' && 'options-active'">Boy</button>
          <button @click="options.gender = 'Unisex'" class="btn"
            :class="options.gender === 'Unisex' && 'options-active'">Unisex</button>
          <button @click="options.gender = 'Girl'" class="btn"
            :class="options.gender === 'Girl' && 'options-active'">Girl</button>
        </div>
      </div>
      <div class="option-container">
        <h4>2) Choose the name's popularity</h4>
        <div class="options-buttons">
          <button @click="options.popularity = 'Trendy'" class="btn"
            :class="options.popularity === 'Trendy' && 'options-active'">Trendy</button>
          <button @click="options.popularity = 'Unique'" class="btn"
            :class="options.popularity === 'Unique' && 'options-active'">Unique</button>
        </div>
      </div>
      <div class="option-container">
        <h4>3) Choose name's length</h4>
        <div class="options-buttons">
          <button @click="options.length = 'Long'" class="btn"
            :class="options.length === 'Long' && 'options-active'">Long</button>
          <button @click="options.length = 'All'" class="btn"
            :class="options.length === 'All' && 'options-active'">All</button>
          <button @click="options.length = 'Short'" class="btn"
            :class="options.length === 'Short' && 'options-active'">Short</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>

interface OptinsState {
  gender: string;
  popularity: string;
  length: string;
}

const options: OptinsState = reactive({
  gender: "Girl",
  popularity: "Unique",
  length: "Short"
})
</script>

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
  border-radius: 2rem;
  padding: 1rem;
  width: 95%;
  margin: 0 auto;
  margin-top: 4rem;
  position: relative;

}

.option-container {
  margin-bottom: 2rem;
}

.btn {
  background: white;
  outline: 0.15rem solid rgb(249, 87, 89);
  padding: 0.75rem;
  width: 12rem;
  font-size: 1rem;
  color: rgb(27, 60, 138);
  cursor: pointer;
  font-weight: 200;
  margin: 1rem;
  border-radius: 1.25rem;

}

.options-active {
  background-color: #ff6262;
  color: white;

}

.options-buttons {}</style>