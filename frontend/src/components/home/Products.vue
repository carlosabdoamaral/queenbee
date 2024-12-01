<script setup lang="ts">
import CaixaATX from "./CaixaATX.vue";
import CaixaATI from "./CaixaATI.vue";
import Racao from "./Racao.vue";
</script>

<template>
    <div class="products-wrapper">
        <div class="section-title">
            <h1>Nosso produto</h1>
            <small>mais recente</small>
        </div>
        <Racao />
        <CaixaATX/>
        <CaixaATI/>
    </div>
</template>