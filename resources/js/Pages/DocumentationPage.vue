<template>
    <BreezePublicLayout>
        <div class="container w-3/4">
            <div class="header">
                <h2 class="featurette-heading">Список <span class="text-muted">документов.</span></h2>
            </div>
            <div class="body mt-4">
                <ol class="list-group list-group-numbered">
                    <li class="list-group-item d-flex justify-content-between align-items-start"
                        v-for="document in documents"
                        :key="document">
                        <div class="icons"><i class="fab fa-accessible-icon"></i></div>
                        <div class="ms-2 me-auto">
                            <div class="fw-bold">{{ document.title }}</div>
                            {{ document.description }}
                        </div>
                        <a :href=document.url target="_blank"><div class="badge rounded-pill download">Скачать .pdf</div></a>
                    </li>
                </ol>
            </div>
        </div>
    </BreezePublicLayout>
</template>

<script>
import BreezePublicLayout from "@/Layouts/Public";
import {Head} from "@inertiajs/inertia-vue3";


export default {
    name: "DocumentationPage",
    components: {
        BreezePublicLayout,
        Head,
    },
    data() {
        return {
            documents: [
                {
                    icon: '',
                    title: 'Сертификат соответствия',
                    description: 'Сертификат подтверждает соответствие характеристик выпускаемой продукции указанным техническим условиям',
                    url: '/docs/sertificate.pdf'
                },
                {
                    icon: '',
                    title: 'Протокол испытаний',
                    description: 'Протокол содержит фактические показатели исследуемых характеристик продукции, исследования проводятся в сертифицированной лаборатории',
                    url: '/docs/protocol.pdf'
                },
                {
                    icon: '',
                    title: 'Инструкция по работе с материалом',
                    description: 'Документ содержит краткое описание продукции, основные характеристики а также порядок работы с материалом, условия хранения и транспортировки',
                    url: '/docs/instruction.pdf'
                },
            ]
        }
    }
}
</script>

<style scoped>
.header {
    margin-top: 80px;
}
.download {
    text-decoration: none;
    background: dodgerblue;
}
.download:hover {
    cursor: pointer;
    background: mediumblue;
}
</style>
