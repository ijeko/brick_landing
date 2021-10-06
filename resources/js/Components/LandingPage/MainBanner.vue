<template>
    <div id="myCarousel" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-indicators">
            <button type="button" data-bs-target="#myCarousel" data-bs-slide-to="0" class=""
                    aria-label="Slide 1"></button>
<!--            <button type="button" data-bs-target="#myCarousel" data-bs-slide-to="1" aria-label="Slide 2" class="active"-->
<!--                    aria-current="true"></button>-->
<!--            <button type="button" data-bs-target="#myCarousel" data-bs-slide-to="2" aria-label="Slide 3"-->
<!--                    class=""></button>-->
        </div>
        <div class="carousel-inner">
            <div class="carousel-item active">
<!--                <svg class="bd-placeholder-img" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg"-->
<!--                     aria-hidden="true" preserveAspectRatio="xMidYMid slice" focusable="false">-->
<!--                    <rect width="100%" height="100%" fill="#777"></rect>-->
<!--                </svg>-->
                <img src="/images/banner/3slide.jpg">

                <div class="container">
                    <div class="carousel-caption text-start">
                        <h1>Диабазовый химическистойкий кирпич.</h1>
                        <p>ТУ 23.69.19.000-001-40980617-2021</p>
                        <p><a class="btn btn-lg btn-primary" href="http://diabazit.ru/catalog/detail/kirpich-diabazovykh-khimicheski-stoykiy/">Подробнее</a></p>
                    </div>
                </div>
            </div>
            <div class="carousel-item">
<!--                <svg class="bd-placeholder-img" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg"-->
<!--                     aria-hidden="true" preserveAspectRatio="xMidYMid slice" focusable="false">-->
<!--                    <rect width="100%" height="100%" fill="#777"></rect>-->
<!--                </svg>-->
                <img src="/images/banner/1slide.jpg">

                <div class="container">
                    <div class="carousel-caption">
                        <h1>Точные размеры и идеальная форма.</h1>
                        <p>Благодаря технологии производства достигается высокая точность размеров и правильность формы.</p>
                        <p><a class="btn btn-lg btn-primary" href="#">Подробнее</a></p>
                    </div>
                </div>
            </div>
            <div class="carousel-item">
<!--                <svg class="bd-placeholder-img" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg"-->
<!--                     aria-hidden="true" preserveAspectRatio="xMidYMid slice" focusable="false">-->
<!--                    <rect width="100%" height="100%" fill="#777"></rect>-->
<!--                </svg>-->
                <img src="/images/banner/2slide.jpg">

                <div class="container">
                    <div class="carousel-caption text-end">
                        <h1>Приемущество в цене.</h1>
                        <p>Цены на диаьбазовый кирпич интереснее чем на керамика, потому что используется местное сырье и высокотехнологичное оборудование.</p>
                        <p><a class="btn btn-lg btn-primary" href="#">Подробнее</a></p>
                    </div>
                </div>
            </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#myCarousel" data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#myCarousel" data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
        </button>
    </div>
</template>

<script>
export default {
    name: 'MainBanner',
    data() {
        return {
            colors: [
                'indigo',
                'warning',
                'pink darken-2',
                'red lighten-1',
                'deep-purple accent-4',
            ],
            slides: [
                'First',
                'Second',
                'Third',
                'Fourth',
                'Fifth',
            ],
        }
    },
}
</script>

<style scoped>

img {
    width:100%;
    object-fit:cover;
}
/* GLOBAL STYLES
-------------------------------------------------- */
/* Padding below the footer and lighter body text */

body {
    padding-top: 3rem;
    padding-bottom: 3rem;
    color: #5a5a5a;
}


/* CUSTOMIZE THE CAROUSEL
-------------------------------------------------- */

/* Carousel base class */
.carousel {
    top: 70px;
    margin-bottom: 4rem;
}

/* Since positioning the image, we need to help out the caption */
.carousel-caption {
    bottom: 3rem;
    z-index: 10;
}

/* Declare heights because of positioning of img element */
.carousel-item {
    height: 32rem;
}

.carousel-item > img {
    position: absolute;
    top: 0;
    left: 0;
    min-width: 100%;
    height: 32rem;
}


/* RESPONSIVE CSS
-------------------------------------------------- */

@media (min-width: 40em) {
    /* Bump up size of carousel content */
    .carousel-caption p {
        margin-bottom: 1.25rem;
        font-size: 1.25rem;
        line-height: 1.4;
    }
}

</style>
