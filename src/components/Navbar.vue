<script setup>
import { onMounted, ref } from 'vue';
const scrollPosition = ref(null);

const updateScroll = () => {
    scrollPosition.value = window.scrollY
};


onMounted(() => {
    window.addEventListener('scroll', updateScroll);
})

</script>
<template>
    <div :class="['navbar', { 'change__color': scrollPosition > 50 }]">
        <div class="container">
            <nav class="navbar-wrapper">
                <div class="navbar__logo">
                    <img src="/images/logo.png" alt="">
                </div>
                <div class="navbar__links">
                    <router-link class="navbar__link" to="#">Главная</router-link>
                    <router-link class="navbar__link" to="#">Преимущества</router-link>
                    <router-link class="navbar__link" to="#">Отзывы</router-link>
                    <router-link class="navbar__link" to="#">Контакты</router-link>
                </div>
                <div class="navbar-wrapper__link">
                    <router-link class="navbar__btn" to="#">Связаться с нами</router-link>
                </div>
            </nav>
        </div>
    </div>
</template>


<style lang="scss">
.navbar {
    position: fixed;
    top: 0;
    right: 0;
    left: 0;
    padding: 15px 0;
    background: transparent;
    z-index: 111;
    transition: all 0.5s;

    &.change__color {
        background-color: #fff;
        box-shadow: 0 0 4px rgb(120 37 141 / 15%);

        .navbar-wrapper {
            &__link {
                background: linear-gradient(87.53deg, #236AD5 29.75%, #23D5D5 100%);

                .navbar__btn {
                    background: #fff;
                    -webkit-background-clip: text;
                }

            }
        }
    }


    &-wrapper {
        display: flex;
        justify-content: space-between;

        &__link {
            padding: 16px 30px;
            background: #FFFFFF;
            border-radius: 16px;
        }
    }

    &__logo {
        img {
            width: 100%;
            height: 100%;
            object-fit: contain;
        }
    }

    &__links {
        display: flex;
        align-items: center;
    }

    &__link {
        font-family: 'Poppins';
        font-weight: 500;
        font-size: 16px;
        line-height: 24px;
        background: linear-gradient(87.53deg, #236AD5 29.75%, #23D5D5 100%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
        cursor: pointer;
        transition: all 0.3s;

        &:not(:last-child) {
            margin-right: 40px;
        }

        &:hover {
            transform: translateY(-15%);
        }

    }

    &__btn {
        font-family: 'Poppins';
        font-weight: 600;
        font-size: 16px;
        line-height: 24px;
        background: linear-gradient(87.53deg, #236AD5 29.75%, #23D5D5 100%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
        padding: 16px 30px;
        border: 1px solid transparent;
        border-radius: 16px;
        cursor: pointer;
    }
}
</style>