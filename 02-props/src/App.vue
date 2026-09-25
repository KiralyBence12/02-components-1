<script setup>
    import MainNavigation from './components/MainNavigation.vue';
    import SiteContent from './components/SiteContent.vue';
    import SiteFooter from './components/SiteFooter.vue';
</script>

<template>
    <header>
        <MainNavigation />
    </header>

    <main>
        <!-- sitecontent komponens használata -->
        <SiteContent/>
    </main>

    <footer>
        <!-- sitefooter komponens használata -->
        <SiteFooter/>
    </footer>
</template>

<style scoped>
</style>
