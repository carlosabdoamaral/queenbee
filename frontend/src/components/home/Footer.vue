<template>
    <div class="footer">
        <div class="custom-col custom-col-logo"><img src="../../assets/logo.png" alt=""></div>

        <div class="custom-col">
            <ul>
                <li><a href="#about">Quem somos</a></li>
                <li><a href="#products">Produtos</a></li>
                <li><a href="#contact">Contato</a></li>
            </ul>
        </div>
        <div class="custom-col">
            <ul>
                <li><a href="https://www.instagram.com/q_ue_enbee/" target="_blank">Instagram</a></li>
                <li><a href="mailto:queenbeehoney60@gmail.com">E-mail</a></li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
$heroHeight: 50dvh;
$accent: #ffc400;
$comp: #3c2300;

.footer {
    min-height: 25dvh;
    background: $comp;
    padding: 1em;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    gap: 16px;

    .custom-col {
        width: calc((100% - 30%)/ 3);
        height: 100%;

        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;

        img {
            width: calc(100% - 20%) !important;

        }

        ul {
            li {
                list-style: none;

                a {
                    color: #FFF7;
                    font-weight: 200;
                    text-decoration: none;
                    font-size: 1.3rem;
                    transition: .2s ease-in-out;
                }

                a:hover {
                    color: #FFF;
                    transition: .2s ease-in-out;
                }
            }
        }
    }
}

@media (max-width: 768px) {
    .footer {

        .custom-col-logo {
            display: none;
        }

        .custom-col {
            width: calc((100% - 30%)/ 2);
        }
    }
}
</style>