<template>
 <div id="app">
     <div class="load" v-if="loadingProgress < 100">
       <LoaderSection :progress="loadingProgress" />
     </div>
     <div v-else>
       <Header/>
   <HeroComponent/>
     </div>


 </div>


</template>

<script>
import LoaderSection from "@/LoaderSection";
import Header from "@/components/Header";
import HeroComponent from "@/components/HeroComponent";
export default {
  name: 'App',
  components: { 
    LoaderSection,
    Header,
    HeroComponent,
  },
 data() {
    return {
      loadingProgress: 0,
      isLoading: true
    };
  },
  created() {
    const simulateLoading = () => {
    const interval = setInterval( () => {
      if (this.loadingProgress >= 100) {
        clearInterval(interval);
        this.isLoading = false;
      } else {
        this.loadingProgress += 10;
      }
    }, 500);
  };

  simulateLoading();
}

};
</script>

<style>
.load {
  position: absolute;
  top: 50%;
  left: 50%;
  right: 600px;
  bottom: 50%;
  text-align: center;
}
</style>
