<script setup>
import Header from '../components/Header.vue';
import PageTitle from '../components/PageTitle.vue';
import Footer from '../components/Footer.vue';
</script>

<template>
    <Header />
    <div class="container">
        <PageTitle :name="Contact us" />
        <div class="map">
            <img src="@/assets/map.png" alt="map">
        </div>
    </div>
    <Footer/>
</template>

<style scoped>
.container {
    margin-top: 96px;
}

.map {
    width: 100%;
    height: 80vh;
    display: flex;
    justify-content: center;
    align-items: center;
    align-content: center;
}
</style>