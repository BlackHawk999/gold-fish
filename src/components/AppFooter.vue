<script setup>
import AppLink from './AppLink.vue';
</script>

<template>
    <div class="footer">
        <div class="container">
            <div class="footer-wrapper">
                <div class="footer__logo">
                    <img src="/images/logo.png" alt="">
                </div>
                <div class="footer-links">
                    <router-link class="footer__link" to="#">Главная</router-link>
                    <router-link class="footer__link" to="#">Отзывы</router-link>
                    <router-link class="footer__link" to="#">Контакты</router-link>
                </div>
                <div class="footer-apps">
                    <app-link />
                </div>
            </div>
        </div>
    </div>
</template>


<style lang="scss">
.footer {
    padding: 37px 0;
    border-top: 1px solid #a5a5a5;

    &-wrapper {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    &__link {
        font-family: 'Poppins';
        font-weight: 500;
        font-size: 16px;
        line-height: 24px;
        color: #000000;
        text-decoration: none;

        &:not(:last-child) {
            margin-right: 64px;
        }
    }
}
</style>