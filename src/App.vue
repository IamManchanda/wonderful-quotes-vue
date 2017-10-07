<template>
  <div class="grid-container">
    <div class="grid-x grid-margin-x grid-padding-y">
      <div class="cell">
        <button class="button alert rounded small" 
                @click="selectedComponent = 'AppRevolution'">Revolution</button>
        <button class="button primary rounded small" 
                @click="selectedComponent = 'AppWomenPower'">Women Power</button>
        <keep-alive>
          <component :is="selectedComponent"></component>
        </keep-alive>
      </div>
    </div>
  </div>
</template>

<script>
import AppRevolution from './components/AppRevolution.vue';
import AppWomenPower from './components/AppWomenPower.vue';

export default {
  data() {
    return {
      selectedComponent: 'AppRevolution'
    };
  },
  components: { AppRevolution, AppWomenPower }
}
</script>

<style lang="scss">
  
</style>
