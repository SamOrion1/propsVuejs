<template>
<header>
  <div class="hello">
    <h1>{{ ordre }}</h1>
    <h1>{{ chiffre }}</h1>
    <h1>{{ ordre1 }}</h1>
    <h1>{{ chiffre1 }}</h1>
    <button @click="clickedButton()">Add 1</button>
  </div>
</header>
</template>

<script lang="ts">

import { Options, Vue } from 'vue-class-component';

@Options({
  props: {
    ordre: String,
    chiffre: String,
    ordre1: String,
    chiffre1: String,
  }
})
export default class Enfant extends Vue {
  ordre!: string
  chiffre!: number
  ordre1!: string
  chiffre1!: number

  public clickedButton(){
    console.log("enfant")
    this.$emit('sam', true)
    }
}
</script>