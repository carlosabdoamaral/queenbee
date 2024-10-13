<template>
    <div class="quote-wrapper">
        <span>"</span>
        <p>Se as abelhas desaparecerem da face da Terra, a humanidade terá apenas mais quatro anos de existência. Sem
            abelhas não há polinização, não há reprodução da flora, sem flora não há animais, sem animais, não haverá
            raça
            humana.
        </p>
        <h3>Albert Einstein</h3>
    </div>
</template>

<style lang="scss" scoped>
.quote-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    min-height: 30dvh;

    span {
        font-size: 4rem;
        font-family: 'Ruge Boogie';
        line-height: .5em;
    }

    p {
        text-align: center;
        font-size: 1.75rem;
        width: 50%;
    }

    h3 {
        font-weight: 200;
    }
}

@media (max-width: 768px) {
    .quote-wrapper {
        p {
            width: 80%;
        }
    }
}

@media (max-width: 425px) {
    .quote-wrapper {
        p {
            font-size: 1.5rem;
        }
    }
}
</style>