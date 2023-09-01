<template>
    <div data-bs-spy="scroll" data-bs-target="cabecalho" data-bs-smooth-scroll="true">
        <section id="carousel">
            <div class="carousel slide" data-bs-ride="carousel">
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
        </section>
    </div>
</template>

<style scoped>
.carousel-inner img {
    height: auto;
    max-width: 100%;
}

@media screen and (max-width: 767px) {
    .carousel-item img {
        height: 280px;
    }

}
</style>