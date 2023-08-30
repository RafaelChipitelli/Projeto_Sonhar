<template>
    <div data-bs-spy="scroll" data-bs-target="cabecalho" data-bs-smooth-scroll="true">
        <section id="sobre-o-restaurante" class="bg-light">
            <div class="carousel slide" data-bs-ride="carousel" id="carousel">
                <div class="carousel-inner">
                    <div class="carousel-item active" data-bs-interval="5000">
                        <img class="d-block w-100"
                            src="https://images.pexels.com/photos/6647037/pexels-photo-6647037.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
                            alt="Foto do Espaço interno do restaurante" />
                    </div>
                    <div class="carousel-item" data-bs-interval="5000">
                        <img class="d-block w-100"
                            src="https://images.pexels.com/photos/6646967/pexels-photo-6646967.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
                            alt="Duas taças de vinho" />
                    </div>
                    <div class="carousel-item" data-bs-interval="5000">
                        <img class="d-block w-100"
                            src="https://images.pexels.com/photos/6646952/pexels-photo-6646952.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
                            alt="Mesa com comida" />
                    </div>
                </div>
                <button class="carousel-control-prev" type="button" data-bs-target="#carousel" data-bs-slide="prev">
                    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Anterior</span>
                </button>
                <button class="carousel-control-next" type="button" data-bs-target="#carousel" data-bs-slide="next">
                    <span class="carousel-control-next-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Próximo</span>
                </button>
                <div class="carousel-indicators">
                    <button class="active" type="button" data-bs-target="#carousel" data-bs-slide-to="0"></button>
                    <button type="button" data-bs-target="#carousel" data-bs-slide-to="1"></button>
                    <button type="button" data-bs-target="#carousel" data-bs-slide-to="2"></button>
                </div>
            </div>
            <div class="pt-5 pb-5">
                <div class="container">
                    <div class="row">
                        <div class="col-md-5">
                            <img src="https://images.pexels.com/photos/6647017/pexels-photo-6647017.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" class="d-block w-100 rounded mb-2" alt="Foto do espaço interno do restaurante">
                        </div>
                        
                        <div class="col-md-7 mt-1 mt-md-0">
                            <h2 class="section-title">Sobre o<span> Instituto</span></h2>
                            <p>
                                Lorem ipsum dolor sit amet consectetur adipisicing elit. Expedita asperiores iure quisquam repudiandae atque! Distinctio eum, vitae atque eligendi aliquid, ea porro blanditiis nemo dolor illum pariatur doloribus perferendis quis.
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<script setup>
</script>

<style scoped>
.carousel-inner img {
    height: auto;
    max-width: 100%;
}

body {
    font-family: Roboto, sans-serif;
}

.section-title {
    font-family: Roboto, sans-serif;
}

.section-title span {
    color: #e15f41;
}

@media screen and (max-width: 767px) {
    .carousel-item img {
        height: 280px;
    }
    
}
</style>
