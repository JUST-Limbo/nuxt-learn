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
export default {
    name: "CommonLayout",
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
