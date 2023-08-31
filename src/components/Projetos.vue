<script setup>
const props = defineProps(['tarefas']);
</script>

<template>
    <div data-bs-spy="scroll" data-bs-target="cabecalho" data-bs-smooth-scroll="true">
        <section id="projetos" class="padding-top pb-5">
            <div class="container">
                <div class="row">
                    <h2 class="section-title text-center">Nossos <span>Projetos</span></h2>
                </div>
                <div class="row mt-3">
                    <div class="col-md-4">
                        <img src="https://images.pexels.com/photos/6995247/pexels-photo-6995247.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="" class="d-block w-100 rounded mb-3">
                        <h3 class="fs-4 text-colored section-title text-center">
                            <i class="bi bi-calendar-heart-fill"></i>
                            Doações de Comida
                        </h3>
                        <p>
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam, vitae. Voluptatem, beatae? Porro optio, ducimus repellendus veniam natus a quia laborum nam quaerat quod perspiciatis eaque! Ad consectetur maiores veniam.
                        </p>
                    </div>
                    <div class="col-md-4">
                        <img src="https://images.pexels.com/photos/6995247/pexels-photo-6995247.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="" class="d-block w-100 rounded mb-3">
                        <h3 class="fs-4 text-colored section-title text-center">
                            <i class="bi bi-arrow-through-heart-fill"></i>
                            BlaBlaBla
                        </h3>
                        <p>
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam, vitae. Voluptatem, beatae? Porro optio, ducimus repellendus veniam natus a quia laborum nam quaerat quod perspiciatis eaque! Ad consectetur maiores veniam.
                        </p>
                    </div>
                    <div class="col-md-4">
                        <img src="https://images.pexels.com/photos/6995247/pexels-photo-6995247.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="" class="d-block w-100 rounded mb-3">
                        <h3 class="fs-4 text-colored section-title text-center">
                            <i class="bi bi-people-fill"></i>
                            Descriminalização
                        </h3>
                        <p>
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam, vitae. Voluptatem, beatae? Porro optio, ducimus repellendus veniam natus a quia laborum nam quaerat quod perspiciatis eaque! Ad consectetur maiores veniam.
                        </p>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<style scoped>

.padding-top {
    padding-top: 6rem;
}

.section-title span {
    color: #e15f41;
}
.text-colored {
    color: #e15f41;
}

/* @media screen and (max-width: 767px) {
    section #eventos {
        padding-top: 1px;
    }
    
} */


</style>