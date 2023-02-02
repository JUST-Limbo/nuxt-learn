<template>
    <div class="App-main">
        <HeaderView />
        <main class="main-content">
            <nuxt />
        </main>
        <FooterView />
    </div>
</template>

<script>
import HeaderView from "@/components/HeaderView.vue";
import FooterView from "@/components/FooterView.vue";

export default {
    name: "CommonLayout",
    components: {
        HeaderView,
        FooterView,
    },
};
</script>

<style lang="scss">
.App-main {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    .main-content {
        flex: 1;
        background-color: #fff;
    }
}
</style>
