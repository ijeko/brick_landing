<template>
    <BreezePublicLayout>
        <div class="container w-3/4">
            <div class="header">
                <h2 class="featurette-heading">Защита прав <span class="text-muted">собственности.</span></h2>
            </div>
            <div class="body mt-4">
                Все права на любые материалы, размещенные на данном ресурсе принадлежат ООО "Диабаз", любое копирование и использльзование без согласия правообладателя запрещеноо.
            </div>
        </div>
    </BreezePublicLayout>
</template>

<script>
import BreezePublicLayout from "@/Layouts/Public";
import {Head} from "@inertiajs/inertia-vue3";


export default {
    name: "Privacy",
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
