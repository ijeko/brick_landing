<template>
    <div class="card bg-dark text-white border-0">
        <img src="/images/waterproof-bg.jpg" class="card-img" alt="...">
        <div class="card-img-overlay">
            <h5 class="card-title font-bold">Водопроницаемость не мнее 24 часов</h5>
            <p class="card-text font-bold">Высокие гидрофобные свойства позволяют применять кирпич <br> в различных жидких средах</p>
            <p class="card-text"></p>
        </div>
    </div>
</template>

<script>
export default {
    name: "CardImage"
}
</script>

<style scoped>
.card-img {
    width: 100%;
    height: 400px;
    object-fit: cover;
}
</style>
