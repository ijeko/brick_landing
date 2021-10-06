<template>
    <footer>
        <nav class="navbar navbar-expand-md navbar-dark fixed-bottom bg-white">
            <div class="container">
        <p>© 2009–2021 ООО "Диабаз" · <a href="/privacy">Защита прав</a> · <a href="#">Условия</a></p>
                <p class="float-end"><a href="#">На верх</a></p>

            </div>
        </nav>
    </footer>
</template>

<script>
export default {
    name: "Footer"
}
</script>

<style scoped>
.fixed-bottom {
    position: fixed;
    bottom: 0;
    right: 0;
    left: 0;
    z-index: 1030;
    height: 70px;
    opacity: 0.8;
}
</style>
