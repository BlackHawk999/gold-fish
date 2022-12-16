<script setup>
import GlobalBtn from "./GlobalBtn.vue";

</script>
<template>
    <div class="monetization">
        <div class="container">
            <div class="monetization-wrapper">
                <div class="monetization-texts">
                    <h3 class="monetization__title">Система <b>монетизации</b></h3>
                    <p class="monetization__text">Заработывайте коины в нашем телеграм-боте, а затем тратьте в играх, и
                        наоборот - за прохождение уровней, вы зарабатываете коины и можете тратить на минуты, смс,
                        мегабайты и ценные призы в <b> Oltin Baliq.</b>
                    </p>
                    <global-btn />
                </div>
                <div class="monetization__img">
                    <img src="/images/monetization-img.png" alt="">
                </div>
            </div>
        </div>
    </div>
    <div class="monetization white">
        <div class="container">
            <div class="monetization-wrapper reverse">
                <div class="monetization-texts">
                    <h3 class="monetization__title">Телеграм <b>Бот</b></h3>
                    <p class="monetization__text">Полный функционал мобильного приложения <b>Oltin Baliq</b> доступен в
                        телеграм-боте. Заходите с любого устройства для того, чтобы получать ежедневные бонусы, а так же
                        совершать покупки в магазине за заработанные коины.
                    </p>
                    <global-btn />
                </div>
                <div class="monetization__img tel">
                    <img src="/images/monetization-bot.png" alt="">
                </div>
            </div>
        </div>
    </div>
    <div class="monetization">
        <div class="container">
            <div class="monetization-wrapper">
                <div class="monetization-texts">
                    <h3 class="monetization__title">Оффлайн <b>доступ</b></h3>
                    <p class="monetization__text">Сервисом <b>Oltin Baliq</b> легко пользоваться с любого устройства.
                        Весь
                        функционал приложения доступен через USSD запрос.
                    </p>
                    <a class="monetization__tel" href="tel:+998910133564">
                        <svg width="40" height="40" viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M15.4323 16.4622C15.4323 16.4622 15.4323 16.4622 15.4323 16.4622L15.4487 16.459C15.4432 16.4601 15.4378 16.4611 15.4323 16.4622ZM16.7482 16.6015L16.7476 16.5995L18.4682 13.1583C18.89 12.3148 18.8684 11.3176 18.4108 10.4933L16.4134 6.8953C15.9095 5.98788 14.9532 5.4248 13.9151 5.4248H9.77348C6.89849 5.4248 4.68963 8.13937 5.65454 10.9991C7.04829 15.1297 9.75782 21.7371 14.0102 25.9894C18.2625 30.2418 24.8699 32.9513 29.0006 34.345C31.8603 35.31 34.5748 33.1011 34.5748 30.2261V26.0839C34.5748 25.0465 34.0126 24.0904 33.1057 23.5863L29.4976 21.5804C28.673 21.1219 27.6751 21.1001 26.8311 21.5221L23.3877 23.2426C23.1239 23.1664 22.7415 23.041 22.2908 22.8489C21.3845 22.4627 20.2325 21.8201 19.206 20.7936C18.1793 19.767 17.5341 18.6122 17.1453 17.7027C16.9519 17.2504 16.8253 16.8666 16.7482 16.6015Z"
                                fill="#333333" />
                        </svg>
                        *718#
                    </a>
                </div>
                <div class="monetization__img">
                    <img src="/images/monetization-call.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>


<style lang="scss">
.monetization {
    background: #F2FBFD;

    &.white {
        background-color: #fff;
    }

    &-wrapper {
        display: flex;
        align-items: center;
        padding-top: 95px;
        padding-bottom: 100px;

        &.reverse {
            flex-direction: row-reverse;
        }
    }

    &__title {
        font-family: 'Poppins';
        font-weight: 600;
        font-size: 32px;
        line-height: 40px;
        color: #333333;

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
        width: 65%;
        margin-top: 16px;
        margin-bottom: 50px;

        b {
            background: linear-gradient(87.53deg, #236AD5 29.75%, #23D5D5 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            text-fill-color: transparent;
        }
    }

    &__img {
        &.tel {
            margin-right: 140px;
        }
    }

    &__tel {
        display: inline-flex;
        align-items: center;
        padding: 24px 40px;
        background: #FFFFFF;
        border-radius: 16px;
        text-decoration: none;
        font-family: 'Poppins';
        font-weight: 500;
        font-size: 32px;
        line-height: 40px;
        color: #333333;
        transition: all 0.3s;

        &:hover {
            background: linear-gradient(87.53deg, #236AD5 29.75%, #23D5D5 100%);
            color: #fff;

            svg path {
                fill: #fff;
            }
        }

        svg {
            width: 100%;
            height: 100%;
            object-fit: contain;
            margin-right: 16px;
        }

    }
}
</style>