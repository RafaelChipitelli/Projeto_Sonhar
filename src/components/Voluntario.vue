<template>
    <section id="contato">
        <div class="container">
            <h2>Cadastre-se Aqui:</h2>
            <form @submit.prevent="handleSubmit">
                <div class="form-campo">
                    <label for="nome">Nome Completo:</label>
                    <input v-model="formData.nome" type="text" id="nome" name="nome">
                </div>
                <div class="form-campo">
                    <label for="CPF">CPF:</label>
                    <input v-mask="'(###) ###.###-###'" v-model="cpf" placeholder="CPF">
                </div>
                <div class="form-campo">
                    <label for="telefone">Telefone:</label>
                    <input v-mask="'(##) #####-####'" v-model="telefone" placeholder="Telefone">
                </div>
                <div class="form-campo">
                    <label for="email">E-mail:</label>
                    <input v-model="formData.email" type="email" id="email" name="email">
                </div>
                <div class="form-campo">
                    <label for="endereço">Endereço Completo:</label>
                    <input v-model="formData.endereço" type="text" id="endereço" name="endereço">
                </div>
                <div class="form-campo">
                    <label for="CEP">CEP:</label>
                    <input v-mask="'#####-###'" v-model="cep" placeholder="CEP">
                </div>
                <button type="submit">Enviar</button>
            </form>
        </div>
    </section>
</template>

<script setup>
import { ref } from 'vue';

const formData = ref({
    nome: '',
    CPF: '',
    telefone: '',
    email: '',
    endereço: '',
    CEP: ''
});

// Definindo as máscaras
const phoneMask = '(00) #####-####';
const cpfMask = '###.###.###-##';
const cepMask = '#####-###';

const handleSubmit = () => {
    // Use a lógica do Vue para manipular o formulário
    // Por exemplo, você pode enviar os dados usando fetch ou axios.
    console.log(formData.value); // Para verificar se os dados estão sendo coletados corretamente
};
</script>

<style scoped>
* {
    margin: 0;
    padding: 0;
    font-family: Roboto, sans-serif;
}

html {
    overflow-x: hidden;
}

.container {
    max-width: 1024px;
    width: 100%;
    margin: 0 auto;
}

header, footer {
    background-color: #192a56;
    padding-top: 16px;
    color: #fff;
}

header {
    position: sticky;
    top: 0;
    left: 0;
    z-index: 1;
}

h2 {
    margin-bottom: 16px;
}

footer {
    position: sticky;
    bottom: 0;
    left: 0;
    z-index: 1;
}

header > .container {
    justify-content: center;
    align-items: center;
    padding-bottom: 16px;
}

footer > .container {
    justify-content: space-between;
    align-items: center;
    padding-bottom: 16px;
}

.container-flex {
    display: flex;
}

section {
    padding: 48px 0;
}

button {
    width: 100%;
    padding: 8px 0;
    border: none;
    background-color: #119759;
    color: #fff;
    font-size: 16px;
    font-weight: bold;
    font-style: italic;
    cursor: pointer;
    border-radius: 6px;
    margin-top: 16px;
    max-width: 120px;
}

.form-campo {
    margin-bottom: 16px;
}

.form-campo label {
    font-weight: bold;
}

.form-campo input,
.form-campo textarea {
    width: 100%;
    padding: 8px;
}

form {
    justify-content: center;
    align-items: center;
    padding-bottom: 16px;
    max-width: 360px;
}

@media (max-width: 767px) {
    form {
        width: 80%; /* Conteúdo com 80% da largura da tela */
        max-width: none; /* Removendo a largura máxima anterior */
        margin: 0 auto; /* Centralizar horizontalmente */
    }

    .form-campo input,
    .form-campo textarea {
        width: 100%; /* Defina a largura dos campos para 100% */
        box-sizing: border-box; /* Adicione isso para garantir que o padding não aumente o tamanho total */
    }
}


</style>