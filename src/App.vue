<template>
    <div id="app">
        <SearchBar class="search-bar"/>
        <div class="launcher-container">
            <LauncherBar class="launcher-bar"/>
        </div>
    </div>
</template>

<script>
    import SearchBar from './components/SearchBar'
    import LauncherBar from './components/LauncherBar'

    export default {
        name: 'app',
        components: {SearchBar, LauncherBar}
    }
</script>

<style lang="less" scoped>
    #app {
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        position: absolute;
        font-family: 'Microsoft YaHei', 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        background-size: cover;
        background-color: #45545D;
        background-image: url("./assets/background.png");

        .search-bar {
            width: 40%;
            margin: 10% auto;
        }

        .launcher-container {
            left: 0;
            right: 0;
            bottom: 3.5%;
            position: fixed;
            display: flex;
            align-items: center;
            justify-content: center;
        }
    }
</style>
