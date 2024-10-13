<script setup lang="ts">
const onChange = (current: number) => {
    console.log(current);
};
</script>

<template>
    <div class="hero">
        <a-carousel :after-change="onChange">
            <div class="hero-img-wrapper">
                <img src="../../../src/assets/hero_01.webp" />
            </div>
            <div class="hero-img-wrapper">
                <img src="../../../src/assets/hero_02.jpeg" />
            </div>
            <div class="hero-img-wrapper">
                <img src="../../../src/assets/hero_03.jpg" />
            </div>
        </a-carousel>
        <div class="backdrop"></div>
        <div class="hero-title">
            <small>Meliponário</small>
            <h1 class="title">Queen<span>Bee</span></h1>
        </div>
    </div>
</template>

<style lang="scss" scoped>
$heroHeight: 60dvh;
$accent: #ffc400;

.hero {
    height: $heroHeight;
    width: 100dvw;

    .hero-title {
        position: relative;
        z-index: 2;
        bottom: 160%;
        text-align: center;
        height: 100%;
        width: 100%;

        color: #FFF;

        small {
            font-size: 1.4rem;
            font-weight: 300;
        }

        h1 {
            font-size: 4rem;
        }

        .title {
            span {
                color: $accent;
            }
        }
    }

    .backdrop {
        position: relative;
        z-index: 1;
        bottom: 100%;
        height: 100%;
        width: 100%;
        background-color: #0006;
    }

    .hero-img-wrapper {
        img {
            height: $heroHeight;
            width: 100%;
            object-fit: cover;
        }
    }

}
</style>