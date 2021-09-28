<template>
    <div 
        v-show="appState == 2" 
        class="bookmaker-vote-wrapper" 
        v-for="(bk, bkIndex) in bookmakersVote" 
        :key="bk.id" 
        :class="bkIndex % 2 == 0 ? 'even' : 'odd'">
    </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({})
export default class App extends Vue {
    private bookmakersVote = [];
}
</script>