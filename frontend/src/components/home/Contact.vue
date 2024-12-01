<script setup lang="ts">
import { ref } from 'vue';

const fullname = ref<string>('');
const email = ref<string>('');
const school = ref<string>('');
const classname = ref<string>('');
const date = ref<string>('');
const message = ref<string>('');

</script>

<template>
    <div class="contact-wrapper">
        <div class="section-title">
            <h1>Agende sua visita</h1>
            <small>e deixe o dia dos alunos mais doce</small>
        </div>
        <div class="contact-form">
            <form action="https://formsubmit.co/carlosabdoamaral@gmail.com" method="post">
                <input type="hidden" name="_subject" value="Novo contato! 🐝✨">
                <input type="hidden" name="_captcha" value="false">
                <input type="hidden" name="_template" value="box">
                <input type="hidden" name="_next" value="https://queenbee-floripa.web.app/">

                <a-row style="width: 100%;">
                    <a-col :span="12" class="col">
                        <a-input v-model:value="fullname" placeholder="Nome completo*" name="Nome completo" required />
                    </a-col>
                    <a-col :span="12" class="col">
                        <a-input v-model:value="email" type="email" placeholder="E-mail*" name="E-mail" required />
                    </a-col>
                </a-row>

                <a-row style="width: 100%;">
                    <a-col :span="8" class="col">
                        <a-input v-model:value="school" placeholder="Nome da escola*" name="Escola" required />
                    </a-col>
                    <a-col :span="8" class="col">
                        <a-input v-model:value="classname" placeholder="Turma*" name="Turma" required />
                    </a-col>
                    <a-col :span="8" class="col">
                        <a-input v-model:value="date" type="date" placeholder="Selecione a data*" name="Data da visita"
                            required />
                    </a-col>
                </a-row>

                <a-row style="width: 100%;">
                    <a-col :span="24" class="col">
                        <a-textarea v-model:value="message" placeholder="Mensagem" :rows="5" name="Mensagem" />
                    </a-col>
                </a-row>
                <a-row>
                    <button type="submit">Agendar!</button>
                </a-row>
            </form>
        </div>
    </div>
</template>

<style lang="scss" scoped>
$accent: #ffc400;
$comp: #3c2300;

.contact-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    .contact-form {
        width: 50%;

        form {
            width: 100%;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            gap: 1em;

            input,
            textarea,
            .ant-picker {
                height: 100%;
                min-height: 54px;
                border-radius: 10px;
                width: 100%;
            }

            input:hover,
            input:focus,
            textarea:hover,
            textarea:focus,
            .ant-picker:hover,
            .ant-picker:focus {
                border-color: $accent;
            }

            .col {
                padding-left: .5em;
                padding-right: .5em;
            }

            button {
                border: none;
                padding: 1em 3em;
                border-radius: 100em;
                color: $comp;
                background: $accent;
                cursor: pointer;
                transition: .3s ease-in-out;
            }

            button:hover {
                transition: .3s ease-in-out;
                box-shadow: -5px 5px 10px #ffcf8b;
            }

            button:disabled {
                opacity: 50%;
            }

        }
    }
}

@media (max-width: 768px) {
    .contact-wrapper {
        .contact-form {
            width: 80%;
        }
    }
}
</style>