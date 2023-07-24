<script>
export default {
  data() {
    return {
      backgroundColor: "#ffffff", 
    };
  },
  methods: {
    changeBackgroundColor() {
      const randomColor = "#" + Math.floor(Math.random() * 16777215).toString(16);
      this.backgroundColor = randomColor;
    },
  },
};
</script>

<template>

    <nav class="middle">
    <div :style="{ backgroundColor: backgroundColor }">
      <p>Background color: {{ backgroundColor }}</p>
    </div>
    <button @click="changeBackgroundColor">Change Color</button>
      </nav>

</template>


<style>
.middle{
    text-align: center;
}

</style>