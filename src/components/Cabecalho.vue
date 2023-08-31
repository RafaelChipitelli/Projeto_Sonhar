<script setup>

</script>

<template>
    <header class="navbar navbar-expand-lg sticky-top p-4" id="cabecalho">
        <div class="container">
            <h1 class="navbar-brand m-0">Projeto Sonhar</h1>
            <button class="navbar-toggler" data-bs-toggle="collapse" data-bs-target="#menu-navegacao">
                <span class="navbar-toggler-icon"></span>
            </button>
            <nav class="navbar-collapse collapse justify-content-end" id="menu-navegacao">
                <ul class="nav nav-pills d-block d-md-flex pt-2">
                    <li class="nav-item fw-bold">
                        <a class="nav-link" href="#sobre-nos">
                            Sobre Nós
                        </a>
                    </li>
                    <li class="nav-item fw-bold">
                        <a class="nav-link" href="#projetos">
                            Projetos
                        </a>
                    </li>
                    <li class="nav-item fw-bold">
                        <a class="nav-link" href="#membro">
                            Membros
                        </a>
                    </li>
                    <li class="nav-item fw-bold">
                        <a class="nav-link" href="#voluntário">
                            Seja Voluntário!
                        </a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style scoped>
.navbar {
    background-color: #e15f41;
}

#cabecalho .nav .nav-link.active {
    background-color: #fff;
    color: #e15f41;
}

#cabecalho .nav .nav-link,
.navbar-brand,
.navbar-brand:hover {
    color: #fff;
}

.navbar-brand {
    font-family: Roboto, sans-serif;
}

.navbar-toggler {
    background-color: #ffeae6;
}

</style>