<script setup>
import NavBar from './components/NavBar.vue';
import Post from './components/Post.vue';
import ShowHide from './components/ShowHide.vue';
import FooterComponent from './components/FooterComponent.vue';
</script>

<template>
<NavBar />
<nav class="math">
    <h1>Vue Math Operations</h1>
    <p>2 + 2 = {{ 2 + 2 }}</p>
    </nav>
<ShowHide />
<FooterComponent />
<Post />
  
</template>
<style>

</style>
