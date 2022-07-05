<template>
  <div class="home">
    <papa1 ordre = "Range ta chambre !" />
    <papa2 chiffre =2222222 @sam="handleEvent" />
    <div>asfhafhaskfaésfaéjf</div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import papa1 from '@/components/Enfant.vue'; // @ is an alias to /src
import papa2 from '@/components/Enfant.vue';

@Options({
  components: {
    papa1,
    papa2
  },
})
export default class MonsieurPapa extends Vue {public handleEvent(data: any){console.log("parent", data)}}
</script>
