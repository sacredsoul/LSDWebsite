<template>
    <div class="home">
        <swiper :options="swiperOption">
            <swiper-slide>
                <img alt="Alpha logo" src="../assets/alpha_logo.png">
                <h1 class="main-title">{{text}}</h1>
            </swiper-slide>
            <swiper-slide v-for="(slide, index) in swiperSlides" :key="index">
                <h1>{{slide}}</h1>
            </swiper-slide>
            <div class="swiper-pagination" slot="pagination"></div>
        </swiper>
    </div>
</template>

<script>
    import 'swiper/dist/css/swiper.css'
    import { swiper, swiperSlide } from 'vue-awesome-swiper'

    export default {
        name: "Home",
        data() {
            return {
                text: "Hi, I' m LSD",
                swiperOption: {
                    direction : 'vertical',
                    height: window.innerHeight,
                    mousewheel: true,
                    pagination: {
                        el: '.swiper-pagination',
                        // dynamicBullets: true,
                        // type: 'progressbar'
                    },

                },
                swiperSlides: [1, 2, 3, 4, 5]
            }
        },
        components: {
            swiper,
            swiperSlide
        }
    }
</script>

<style scoped>
    .home {
        font-size: 28px;
    }
    .home img {
        margin-top: 60px;
        width: 200px;
        height: 200px;
    }

    .main-title {
        padding-top: 60px;
    }
</style>