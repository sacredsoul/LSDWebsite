<template>
    <div id="app">
        <Home></Home>
    </div>
</template>

<script>
    import Home from './components/Home.vue'

    export default {
        name: 'app',
        components: {
            Home
        }
    }

</script>

<style>
    #app {
        /*font-family: 'Avenir', Helvetica, Arial, sans-serif;*/
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: white;
    }

    body {
        font-family: "Poppins", Arial, sans-serif;
        background: #121212;
        font-size: 18px;
        line-height: 1.8;
        font-weight: 400;
        position: relative;
        margin: 0;
    }

    body:after {
        position: fixed;
        top: -150px;
        right: -50px;
        bottom: 0;
        content: '';
        width: 400px;
        height: 600px;
        border: 2px solid rgba(255, 255, 255, 0.05);
        z-index: -1;
        -webkit-transform: rotate(-30deg);
        -moz-transform: rotate(-30deg);
        -ms-transform: rotate(-30deg);
        -o-transform: rotate(-30deg);
        transform: rotate(-30deg);
    }
    body:before {
        position: fixed;
        top: 500px;
        left: -100px;
        bottom: 0;
        content: '';
        width: 400px;
        height: 400px;
        border: 2px solid rgba(255, 255, 255, 0.05);
        z-index: -1;
        -webkit-transform: rotate(20deg);
        -moz-transform: rotate(20deg);
        -ms-transform: rotate(20deg);
        -o-transform: rotate(20deg);
        transform: rotate(20deg);
    }
</style>
