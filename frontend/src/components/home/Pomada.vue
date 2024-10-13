<template>
    <div class="pomada-wrapper">
        <div class="text-wrapper">
            <h1>Pomada <span>cicatrizante!</span></h1>
            <p>Descubra o poder da natureza com nossa pomada cicatrizante, feita com uma combinação única de babosa e
                mel. A
                babosa, conhecida por suas propriedades regeneradoras, acelera a cicatrização, enquanto o mel, com sua
                ação
                antisséptica e antimicrobiana, protege e hidrata a pele. Juntos, esses ingredientes fazem da nossa
                pomada uma
                solução natural e eficaz para cuidar da sua saúde, promovendo a recuperação da pele de forma segura e
                saudável.
            </p>
            <button>Quero conhecer!</button>
        </div>
        <div class="img-wrapper">
            <img src="../../../src/assets/pote.png" alt="">
        </div>
    </div>

</template>
<style lang="scss" scoped>
$pomadaWrapperHeight: 500px;
$heroHeight: 50dvh;
$accent: #ffc400;
$comp: #3c2300;

.pomada-wrapper {
    text-align: center;
    border-radius: 2em;
    height: $pomadaWrapperHeight;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;

    .text-wrapper {
        width: 50%;
        height: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        text-align: center;
        background-color: $accent;
        color: $comp;

        h1 {
            font-size: 2.5rem;
            font-weight: 400;

            span {
                font-weight: bold;
            }
        }

        p {
            width: 75%;
            font-size: 1.3rem;
            font-weight: 300;
        }

        button {
            margin-top: 2em;
            border: none;
            padding: 1em 3em;
            border-radius: 100em;
            color: $accent;
            background: $comp;
            cursor: pointer;
            transition: .3s ease-in-out;
        }

        button:hover {
            transition: .3s ease-in-out;
            box-shadow: -5px 5px 10px #bd6e00;
        }
    }

    .img-wrapper {
        width: 50%;

        img {
            height: calc($pomadaWrapperHeight - 100px);
            aspect-ratio: 1/1;
        }
    }
}

@media (max-width: 1024px) {
    .img-wrapper {
        display: none;
    }

    .pomada-wrapper {
        flex-direction: column;
        background-color: $accent;
        padding: 1em;
        border-radius: 0;

        .text-wrapper {
            width: 100%;
            background-color: transparent;

            h1 {
                font-size: 2rem;
            }

            p {
                font-size: 1rem;
                width: 90%;
            }
        }
    }
}
</style>