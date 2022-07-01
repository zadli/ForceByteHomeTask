<script setup>
</script>

<template>
    <div class="footer__back">
        <div class="footer">
            <div class="intersted">
                <div class="col">
                    <span>
                        Intersted to work with our team?
                    </span>
                    <span>
                        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut
                        labore
                        et dolore magna aliqua. Ut enim ad minim veniam.
                    </span>
                </div>
                <a href="#" class="link__button">
                    Let’s Talk
                </a>
            </div>
            <img src="@/assets/white_border.svg" />
            <div class="links">
                <div class="cols">
                    <div class="column">
                        <span><svg xmlns="http://www.w3.org/2000/svg" width="48" height="48" viewBox="0 0 48 48"
                                fill="none">
                                <circle cx="16" cy="24" r="16" fill="#98C3E8" />
                                <circle cx="32" cy="24" r="15" fill="white" stroke="#316099" stroke-width="2" />
                                <path
                                    d="M38.3 31L33.38 17H29.96L25.06 31H28.04L28.88 28.48H34.46L35.3 31H38.3ZM31.68 20.18L33.6 25.9H29.76L31.68 20.18Z"
                                    fill="#316099" />
                            </svg>Afrianska</span>
                        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                        <p>+62-812-7313-4321</p>
                        <p>hello.afrian@gmail.com</p>
                    </div>
                    <div class="column">
                        <span>About Us</span>
                        <p>About</p>
                        <p>What we do</p>
                        <p>Project</p>
                        <p>How It Work With Us</p>
                    </div>
                    <div class="column">
                        <span>Follow us</span>
                        <p>Instagram</p>
                        <p>Facebook</p>
                        <p>LinkedIn</p>
                    </div>
                </div>

            </div>
            <div class="copyright">
                <span>
                    2019 © Afrianska. All rights reserved.
                </span>
            </div>
        </div>
    </div>
</template>

<style scoped>
.footer {

    width: calc(90% - 200px);
    height: 87.5vh;
    background-color: #316099;
    border-radius: 0px 200px 0px 0px;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    padding-left: 200px;
    color: white
}

.footer img {
    width: 100%;
    margin-left: -210px;
}

.footer .intersted,
.footer .links {
    display: flex;
    flex-direction: row;
    align-content: center;
    align-items: center;
    height: 50%;
}

.footer .intersted a {
    width: 10%;
    height: 32px;
    font-family: 'Gilroy', sans-serif;
    margin-right: 256px;
    padding: 16px;
    padding-left: 64px;
    padding-right: 64px;
    text-decoration: none;
    color: white;
    background: #5A98D0;
    box-shadow: 5px 10px 20px rgba(53, 110, 173, 0.2);
    border-radius: 10px;
    display: flex;
    justify-content: center;
    align-content: center;
    align-items: center;
}

.footer .col {
    height: 25vh;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: flex-start;
    align-content: start;
}

.footer .intersted .col span:nth-child(1) {
    font-family: 'Gilroy', sans-serif;
    width: 45%;
    font-size: 36px;
    line-height: 46px;
}

.footer .intersted .col span:nth-child(2) {
    width: 60%;
}

.footer .cols {
    width: 80%;
    margin-top: 48px;
    margin-bottom: 48px;
    display: flex;
    flex-direction: row;
}

.footer .cols .column {
    width: 50%;
    display: flex;
    flex-direction: column;

}

.footer .cols .column span {
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    align-items: center;
    align-content: center;
    font-size: 1.5rem;
}

.footer .cols .column span svg {
    margin-right: 16px;
}

.footer .cols .column p {
    width: 70%;
    opacity: 0.7;
}

.footer .cols .column p:nth-child(2) {
    margin-top: 24px;
}

.footer .copyright {
    margin-bottom: 48px;
    opacity: 0.4;
}
</style>