<script setup>
const props = defineProps({
    title: {
        type: String,
        required: true
    },
    image: {
        type: String,
        required: true,
    },
    class: {
        type: String,
        default: '',
    },
})
</script>
<template>
    <div class="prize-card" :class="props.class">
        <p class="prize-card__text">{{ title }}</p>
        <div class="prize-card__img">
            <img :src="image" alt="">
        </div>
    </div>
</template>


<style lang="scss">
.prize-card {
    display: flex;
    justify-content: space-between;
    background: #F2FBFD;
    border-radius: 16px;
    padding: 20px;
    height: 190px;
    transition: 0.3s;
    cursor: pointer;
    
    &:hover {
        box-shadow: -5px 5px 5px rgba($color: #000000, $alpha: 0.5);
        background: linear-gradient(87.53deg, #236AD5 29.75%, #23D5D5 100%);
        transform: scale(1.02) translate(5px, -5px);

        .prize-card__text {
            color: #F2FBFD;
        }

    }

    &.full {
        grid-column: span 2;
    }

    &__text {
        font-family: 'Poppins';
        font-weight: 600;
        font-size: 24px;
        line-height: 36px;
        color: #333333;

    }

    &__img {
        display: flex;
        align-items: flex-end;
    }
}
</style>