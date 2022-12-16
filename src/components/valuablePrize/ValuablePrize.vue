<script setup>
import { reactive } from 'vue';
import PrizeCard from './PrizeCard.vue';

const state = reactive({
    prizes: [
        {
            title: 'Play Station',
            image: '/images/valuable-console.png',
        },
        {
            title: 'Наушники',
            image: '/images/valuable-headphone.png',
        },
        {
            title: 'Телефон',
            image: '/images/valuable-phone.png',
            class: 'full'
        },
        {
            title: 'Ноутбук MacBook Pro',
            image: '/images/valuable-pc.png',
            class: 'full'
        },
        {
            title: 'Мышь',
            image: '/images/valuable-mouse.png',
        },
        {
            title: 'Smart Watch',
            image: '/images/valuable-watch.png',
        },
    ]
});
</script>

<template>
    <div class="valuable">
        <div class="container">
            <div class="valuable-wrapper">
                <h3 class="valuable__title">Ценные <b>призы</b></h3>
                <p class="valuable__subtitle">Вы также можете приобрести ценные товары в нашем маркет-плейсе</p>
                <div class="valuable-items">
                    <prize-card v-for="(item, idx) in state.prizes" :key="idx" :title="item.title" :image="item.image"
                        :class="item.class" />
                </div>
            </div>
        </div>
    </div>
</template>


<style lang="scss">
.valuable {
    padding: 100px 0;
    &__title {
        font-family: 'Poppins';
        font-weight: 600;
        font-size: 32px;
        line-height: 40px;
        text-align: center;
        color: #333333;

        b {
            background: linear-gradient(87.53deg, #236AD5 29.75%, #23D5D5 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            text-fill-color: transparent;
        }
    }

    &__subtitle {
        font-family: 'Poppins';
        font-weight: 500;
        font-size: 16px;
        line-height: 24px;
        text-align: center;
        color: #858585;
        margin-top: 16px;

    }

    &-items {
        display: grid;
        grid-template-columns: auto auto auto auto;
        grid-gap: 20px;
        margin-top: 50px;
    }
}
</style>