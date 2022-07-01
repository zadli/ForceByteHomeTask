<script setup>
import Header from '../components/Header.vue';
import PageTitle from '../components/PageTitle.vue';
import Footer from '../components/Footer.vue';
</script>

<template>
    <Header />
    <div class="container">
        <section class="landing">
            <div class="landing-text">
                <span>New Automation Tool for Your Home</span>
                <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Faucibus tristique vulputate ultrices ut
                    mauris tellus at. Posuere sollicitudin odio tellus elit.</span>
                <a href="#" class="link__button">See Our Project</a>
            </div>
            <img src="@/assets/hero.svg" alt="landing">
        </section>
        <section class="help">

        </section>
        <section class="finished">
            <div class="head">
                <span>Our Finished Projects</span>
                <span>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.</span>
            </div>
            <div class="body">
                <img src="@/assets/pr1.png">
                <img src="@/assets/pr2.png">
                <img src="@/assets/pr3.png">
            </div>
        </section>
        <section class="our__clients">
            <div class="head">
                <span>Our Beloved Client</span>
                <span>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.</span>
            </div>
            <div class="body">
                <span style="border-bottom: 1px solid white;border-right: 1px solid white;">Logo Client 1</span>
                <span style="border-bottom: 1px solid white;border-right: 1px solid white;">Logo Client 1</span>
                <span style="border-bottom: 1px solid white;border-right: 1px solid white;">Logo Client 1</span>
                <span style="border-bottom: 1px solid white">Logo Client 1</span>
                <span style="border-right: 1px solid white;">Logo Client 1</span>
                <span style="border-right: 1px solid white;">Logo Client 1</span>
                <span style="border-right: 1px solid white;">Logo Client 1</span>
                <span style="background-color: #1F3F68;">More Clients</span>
            </div>
        </section>
    </div>
    <Footer/>
</template>

<style scoped>
.container {
    margin-top: 96px;
    width: 100%;
}

.landing {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    height: 100%;
    width: 100%;
}

.landing .landing-text {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    width: 40%;
    height: 100%;
    padding-left: 200px;
}

.landing .landing-text span:nth-child(1) {
    width: 90%;
    font-size: 4rem;
    font-family: 'Galien';
    font-weight: 550;
    color: #1F3F68;
    line-height: 1.3;
}

.landing .landing-text span:nth-child(2) {
    margin-top: 32px;
    width: 80%;
    font-size: 1.3rem;
    color: #1F3F68;
    opacity: 0.6;
}

.landing .link__button {
    font-family: 'Gilroy', sans-serif;
    margin-top: 64px;
    padding: 20px;
    padding-left: 48px;
    padding-right: 48px;
    text-decoration: none;
    color: white;
    background: #5A98D0;
    box-shadow: 5px 10px 20px rgba(53, 110, 173, 0.2);
    border-radius: 10px;

}

.finished {
    width: 100%;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
}

.finished .head {
    margin-left: 256px;
    height: 30vh;
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    align-content: center;
    align-items: center;
}
.finished .head span:nth-child(1) {
    font-size: 2rem;
    color: #1F3F68;
    width: 20%;
}

.finished .head span:nth-child(2) {
    font-size: 1.2rem;
    color: darkgray;
    width: 60%;
}

.finished .body {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    align-content: center;
    align-items: center;
    margin-bottom: 128px;
}

.finished .body img {
    padding: 48px;
}

.our__clients {
    height: 85vh;
    width: 100%;
    background: #5A98D0;
    border-radius: 200px 0px 0px 0px;
}

.our__clients .head {
    margin-left: 256px;
    height: 30vh;
    display: flex;
    flex-direction: row;
    color: white;
    justify-content: flex-start;
    align-content: center;
    align-items: center;
}
.our__clients .head span:nth-child(1) {
    font-size: 2rem;
    width: 20%;
}

.our__clients .head span:nth-child(2) {
    font-size: 1.2rem;
    color: lightgray;
    width: 50%;
}

.our__clients .body {
    margin-top: -96px;
    margin-left: 128px;
    margin-right: 256px;
    width: 80%;
    height: 70vh;
    color: white;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    align-content: center;
}

.our__clients .body span {
    font-size: 1.5rem;
    width: 20%;
    height: 100px;
    padding: 16px;
    display: flex;
    justify-content: center;
    align-items: center;
    align-content: center;
    
}
.footer__back{
    background-color: #5A98D0;
}
</style>