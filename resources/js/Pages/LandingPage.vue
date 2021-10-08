<template>
    <BreezePublicLayout>
<!--        <Header></Header>-->
        <MainBanner></MainBanner>
        <MainBody></MainBody>
    </BreezePublicLayout>
</template>

<script>
import BreezePublicLayout from "@/Layouts/Public";
import {Head} from "@inertiajs/inertia-vue3";
import Header from "@/Components/LandingPage/Header";
import MainBanner from "@/Components/LandingPage/MainBanner";
import MainBody from "@/Components/LandingPage/MainBody";
import CardImage from "@/Components/LandingPage/CardImage";

export default {
    name: "LandingPage",
    components: {
        CardImage,
        MainBody,
        MainBanner,
        Header,
        BreezePublicLayout,
        Head,
    },
}
</script>

<style scoped>

</style>
