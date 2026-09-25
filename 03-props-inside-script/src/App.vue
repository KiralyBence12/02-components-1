<script setup>
    import { ref } from 'vue';

    import MainNavigation from './components/MainNavigation.vue';
    import SiteContent from './components/SiteContent.vue';
    import SiteFooter from './components/SiteFooter.vue';
    import InputField from './components/InputField.vue';

    const title = ref("VUE")

    setTimeout(() => {
        title.value = "REACT"
    }, 2000);   

    function handleInputClick() {
        alert("Input field clicked!");
    }
</script>

<template>
    <header>
        <MainNavigation :title="title"/>
    </header>

    <main>
        <!-- sitecontent komponens használata -->
        <SiteContent/>
        <InputField @on-input="handleInputClick"/>
    </main>

    <footer>
        <!-- sitefooter komponens használata -->
        <SiteFooter/>
    </footer>
</template>

<style scoped>
</style>
