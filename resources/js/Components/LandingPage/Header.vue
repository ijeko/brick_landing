<template>
    <header>
        <nav class="navbar navbar-expand-md navbar-dark fixed-top bg-dark">
            <div class="container-fluid">
                <a class="navbar-brand" href="#">Диабаз</a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarCollapse" aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarCollapse">
                    <ul class="navbar-nav me-auto mb-2 mb-md-0">
                        <li class="nav-item">
                            <a class="nav-link" aria-current="page" href="/">О продукции</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="/documents">Документация</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link disabled">Коммерческое предложение</a>
                        </li>
                    </ul>
<!--                    <form class="d-flex">-->
<!--                        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">-->
<!--                        <button class="btn btn-outline-success" type="submit">Search</button>-->
<!--                    </form>-->
                </div>
            </div>
        </nav>
    </header>
</template>

<script>
export default {
    name: "Header"
}
</script>

<style scoped>
.bg-dark {
    --bs-bg-opacity: 1;
    /*background-color: rgba(var(--bs-dark-rgb),var(--bs-bg-opacity))!important;*/
}
header {
    display: block;
}
.fixed-top {
    position: fixed;
    top: 0;
    right: 0;
    left: 0;
    z-index: 1030;
    height: 70px;
}
</style>
