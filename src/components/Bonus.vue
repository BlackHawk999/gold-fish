<script setup>
import GlobalBtn from './GlobalBtn.vue'

</script>
<template>
    <section>
        <div class="bonus">
            <div class="container">
                <div class="bonus-wrapper">
                    <h3 class="bonus__title">Ежедневные бонусы</h3>
                    <p class="bonus__text">Выполняйте активности в нашем боте или приложении, и зарабатывайте монеты,
                        которые можно потратить на <br /> дополнительные ресурсы в виде мегабайт, минут, СМС, а также
                        приобрести
                        товары в нашем маркет-плейсе
                    </p>
                    <div class="bonus-blocks">
                        <div class="bonus-block" v-for="item in 3" :key="item">
                            <svg width="40" height="40" viewBox="0 0 40 40" fill="none"
                                xmlns="http://www.w3.org/2000/svg">
                                <path
                                    d="M35.8068 16.7118C27.4159 8.75986 14.4967 8.34131 5.6303 15.4575C5.13847 15.8523 4.65894 16.2704 4.19318 16.7118C3.6921 17.1866 2.90092 17.1654 2.42605 16.6643C1.95118 16.1632 1.97243 15.372 2.47351 14.8972C2.98908 14.4086 3.52025 13.9455 4.0654 13.5079C13.8984 5.61585 28.2209 6.07844 37.5265 14.8972C38.0276 15.372 38.0488 16.1632 37.574 16.6643C37.0991 17.1654 36.3079 17.1866 35.8068 16.7118Z"
                                    fill="url(#paint0_linear_35_50)" />
                                <path
                                    d="M7.44945 20.6153C14.3809 13.6838 25.6191 13.6838 32.5506 20.6153C33.0387 21.1035 33.0387 21.8949 32.5506 22.3831C32.0624 22.8712 31.2709 22.8712 30.7828 22.3831C24.8276 16.4279 15.1724 16.4279 9.21722 22.3831C8.72907 22.8712 7.93761 22.8712 7.44945 22.3831C6.9613 21.8949 6.9613 21.1035 7.44945 20.6153Z"
                                    fill="url(#paint1_linear_35_50)" />
                                <path
                                    d="M12.4495 26.0442C16.6195 21.8742 23.3805 21.8742 27.5506 26.0442C28.0387 26.5324 28.0387 27.3239 27.5506 27.812C27.0624 28.3002 26.2709 28.3002 25.7828 27.812C22.589 24.6182 17.411 24.6182 14.2172 27.812C13.7291 28.3002 12.9376 28.3002 12.4495 27.812C11.9613 27.3239 11.9613 26.5324 12.4495 26.0442Z"
                                    fill="url(#paint2_linear_35_50)" />
                                <path
                                    d="M20 33.3334C21.1506 33.3334 22.0833 32.4006 22.0833 31.25C22.0833 30.0995 21.1506 29.1667 20 29.1667C18.8494 29.1667 17.9167 30.0995 17.9167 31.25C17.9167 32.4006 18.8494 33.3334 20 33.3334Z"
                                    fill="url(#paint3_linear_35_50)" />
                                <defs>
                                    <linearGradient id="paint0_linear_35_50" x1="13.204" y1="33.3334" x2="39.3646"
                                        y2="31.7436" gradientUnits="userSpaceOnUse">
                                        <stop stop-color="#236AD5" />
                                        <stop offset="1" stop-color="#23D5D5" />
                                    </linearGradient>
                                    <linearGradient id="paint1_linear_35_50" x1="13.204" y1="33.3334" x2="39.3646"
                                        y2="31.7436" gradientUnits="userSpaceOnUse">
                                        <stop stop-color="#236AD5" />
                                        <stop offset="1" stop-color="#23D5D5" />
                                    </linearGradient>
                                    <linearGradient id="paint2_linear_35_50" x1="13.204" y1="33.3334" x2="39.3646"
                                        y2="31.7436" gradientUnits="userSpaceOnUse">
                                        <stop stop-color="#236AD5" />
                                        <stop offset="1" stop-color="#23D5D5" />
                                    </linearGradient>
                                    <linearGradient id="paint3_linear_35_50" x1="13.204" y1="33.3334" x2="39.3646"
                                        y2="31.7436" gradientUnits="userSpaceOnUse">
                                        <stop stop-color="#236AD5" />
                                        <stop offset="1" stop-color="#23D5D5" />
                                    </linearGradient>
                                </defs>
                            </svg>
                            <h6 class="bonus-block__title">
                                Бонусные MB
                            </h6>
                            <p class="bonus-block__text">Возможность получать интернет трафик каждый день</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="premium-bonus">
            <div class="container">
                <div class="premium-bonus-wrapper">
                    <div class="premium-bonus__img">
                        <img src="/images/premium-bonus.png" alt="">
                    </div>
                    <div class="premium-bonus-texts">
                        <h3 class="premium-bonus__title">Премиум <b> бонусы и пополнение</b></h3>
                        <p class="premium-bonus__text sub">Безграничная возможность выигрывать пополнения вашего
                            баланса.
                        </p>
                        <p class="premium-bonus__text">
                            Уровень 1: 10 000 сум 15 000 сум 20 000 сум <br />
                            Уровень 2: 25 000 сум 30 000 сум 35 000 сум <br />
                            Уровень 3: 40 000 сум 45 000 сум 50 000 сум
                        </p>
                        <div class="premium-bonus__btn">
                            <global-btn />
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>


<style lang="scss">
.bonus {
    padding: 100px 0;
    background-image: url('/images/bonus-bg.png');
    background-repeat: no-repeat;
    background-size: 3% auto;
    background-position: left;

    &__wrapper {
        display: flex;
        flex-direction: column;
    }

    &__title {
        font-family: 'Poppins';
        font-weight: 600;
        font-size: 32px;
        line-height: 40px;
        color: #333333;
        text-align: center;
        margin-bottom: 16px;
    }

    &__text {
        font-family: 'Poppins';
        font-weight: 500;
        font-size: 16px;
        line-height: 24px;
        text-align: center;
        color: #858585;
    }

    &-blocks {
        display: flex;
        align-items: center;
        margin-top: 26px;
    }

    &-block {
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 24px;
        background: #F2FBFD;
        border-radius: 24px;

        &:not(:last-child) {
            margin-right: 30px;
        }

        &__title {
            font-family: 'Poppins';
            font-weight: 600;
            font-size: 20px;
            line-height: 24px;
            color: #333333;
            margin-top: 24px;
            margin-bottom: 16px;
        }

        &__text {
            font-family: 'Poppins';
            font-weight: 500;
            font-size: 16px;
            line-height: 24px;
            text-align: center;
            color: #858585;
            width: 75%;
        }
    }
}

.premium-bonus {
    background-image: url('/images/premium-bonus-bg.png');
    background-repeat: no-repeat;
    background-size: 3% auto;
    background-position: right;

    &-wrapper {
        display: flex;
        align-items: center;
    }

    &-texts {
        display: flex;
        flex-direction: column;
        margin-left: 50px;
    }

    &__title {
        font-family: 'Poppins';
        font-weight: 600;
        font-size: 32px;
        line-height: 40px;
        color: #333333;
        margin-bottom: 16px;

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

        &.sub {
            margin-bottom: 15px;
        }
    }

    &__btn {
        margin-top: 50px;
    }
}
</style>