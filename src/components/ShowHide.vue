<script>

export default {
  data() {
    return {
      showElement: false
    };
  },
  methods: {
    toggleElement() {
      this.showElement = !this.showElement;
    }
  }
};
</script>


<template>
  <div class="math">
    <button @click="toggleElement">{{ showElement ? 'Hide' : 'Show' }}</button>
    <div v-if="showElement">
      <p>You're great at finding the way to "The Button" :D</p>
    </div>
    <div v-else>
        <p>Click me!?</p>
      </div>
  </div>
  
</template>


<style>
.math{
    text-align: center;
}
</style>