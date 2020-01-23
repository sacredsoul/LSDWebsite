<template>
    <div class="home">
        <img alt="Alpha logo" src="../assets/alpha_logo.png">
        <h1 class="main-title">{{text}}</h1>
    </div>
</template>

<script>
    export default {
        name: "Home",
        data() {
            return {
                text: "Hi, I' m LSD"
            }
        }
    }
</script>

<style scoped>
    .home {
        font-size: 28px;
    }
    .home img {
        margin-top: 60px;
        width: 200px;
        height: 200px;
    }

    .main-title {
        padding-top: 60px;
    }
</style>