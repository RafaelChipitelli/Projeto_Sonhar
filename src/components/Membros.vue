<template>
    <section id="membros" class="bg-light py-5">
        <div class="container">
            <h2 class="text-center mb-5">Nossa Equipe</h2>
            <div class="row">
                <div class="col-md-4 mb-4" v-for="(member, index) in members" :key="index">
                    <div class="card">
                        <img  :src="member.photo" class="card-img-top rounded-circle mx-auto d-block" :alt="member.name" />
                        <div class="card-body">
                            <h5 class="card-title">{{ member.name }}</h5>
                            <p class="card-text">{{ member.role }}</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
const members = [
    {
        name: "Fulano da Silva",
        role: "Fundador",
        photo: "https://images.pexels.com/photos/6626882/pexels-photo-6626882.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
    },
    {
        name: "Ciclana Rodrigues",
        role: "Comunicação",
        photo: "https://images.pexels.com/photos/5615665/pexels-photo-5615665.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
    },
    {
        name: "Beltrano Oliveira",
        role: "Financeiro",
        photo: "https://images.pexels.com/photos/7654096/pexels-photo-7654096.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
    }
];
</script>

<style scoped>
.card {
    border: none;
    text-align: center;
}

.card img {
    margin-top: 35px;
}

.card-title {
    margin-top: 10px;
    font-weight: bold;
}

.card-text {
    color: #777;
}

.rounded-circle {
    border-radius: 50%;
    object-fit: cover;
    width: 150px;
    height: 150px;
}
</style>
