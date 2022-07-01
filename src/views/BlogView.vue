<script setup>
import Header from '../components/Header.vue';
import PageTitle from '../components/PageTitle.vue';
import Footer from '../components/Footer.vue';
</script>

<template>
    <Header/>
    <div class="container">
        <PageTitle :name="Blog"/>
    </div>
    <Footer/>
</template>

<style scoped>
.container {
    margin-top: 96px;
}
</style>