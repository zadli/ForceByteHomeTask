<script setup>
props: ['name']
</script>

<template>
<div class="title">
    <span class="title__text">{{this.name}}</span>
    <br/>
    <span class="description">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. </span>
</div>
</template>

<style scoped>
.title {
    width: 100%;
    height: 250px;
    background-image: url("/src/assets/title_back.svg");
    background-size: cover;
    display: flex;
    justify-content: center;
    align-items: center;
    align-content: center;
    flex-direction: column;
}

.title .title__text {
    font-size: 3rem;
    font-weight: bold;
    color: white;
}

.title .description {
    font-size: 1.5rem;
    color: rgba(255, 255, 255, 0.4);
    padding-left: 300px;
    padding-right: 300px;
    text-align: center;
}
</style>