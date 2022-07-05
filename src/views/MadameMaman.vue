<template>
  <div class="home">
    <maman1 ordre1 = "Fais les devoirs !"/>
    <maman2 chiffre1 =888888 />
    <div>830248726428489269428</div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import maman1 from '@/components/Enfant.vue'; // @ is an alias to /src
import maman2 from '@/components/Enfant.vue';

@Options({
  components: {
    maman1,
    maman2
  },
})
export default class MadameMaman extends Vue {}
</script>
