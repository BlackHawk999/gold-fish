<script setup>
import AppLink from "./AppLink.vue";

</script>

<template>
    <div class="intro">
        <div class="container">
            <div class="intro-wrapper">
                <div class="intro-texts">
                    <h1 class="intro__title">
                        <b> Oltin Baliq - </b>приложение для <br /> заработка бонусов!
                    </h1>
                    <p class="intro__text">Oltin Baliq это интерактивная платформа которая позволяет получать мегабайты,
                        минуты и СМС ежедневно на ваш абонентский номер телефона. Режим Oltin Baliq Premium позволяет
                        получать еще больше бонусов, а также ценные призы.
                    </p>
                    <div class="intro-apps">
                        <app-link />
                    </div>
                </div>
                <div class="intro__img">
                    <img src="/images/intro-img.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>


<style lang="scss">
.intro {
    padding: 90px 0;
    min-height: 100vh;
    background-image: url('/images/intro-bg.png');
    background-size: 38% auto;
    background-position: right top;
    background-repeat: no-repeat;

    &-wrapper {
        display: flex;
        align-items: center;
        height: 100%;
    }

    &-texts {
        display: flex;
        flex-direction: column;
    }

    &__title {
        font-family: 'Poppins';
        font-weight: 600;
        font-size: 40px;
        line-height: 60px;

        b {
            background: linear-gradient(87.53deg, #236AD5 29.75%, #23D5D5 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            text-fill-color: transparent;
        }
    }

    &__text {
        font-family: 'Poppins';
        font-weight: 500;
        font-size: 16px;
        line-height: 24px;
        color: #858585;
    }

    &-apps {
        margin-top: 40px;
    }
}
</style>