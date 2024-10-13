<template>
    <div class="header">
        <a href="#about">Quem somos</a>
        <a href="#products">Produtos</a>
        <a href="#contact">Contato</a>
    </div>
</template>

<style lang="scss" scoped>
$headerHeight: 64px;

.header {
    position: sticky;
    z-index: 99999;
    top: 0;
    width: 100%;
    height: $headerHeight;
    background: rgb(60, 35, 0);

    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    gap: 10dvw;

    a {
        color: #FFF7;
        font-weight: 300;
        text-decoration: none;
        font-size: 1.1rem;
        transition: .2s ease-in-out;
    }

    a:hover {
        color: #FFF;
        transition: .2s ease-in-out;
    }
}
</style>