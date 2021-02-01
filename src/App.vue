<template>
    <div id="app">
        <img alt="Vue logo" src="./assets/logo.png" />
        <HelloWorld msg="Welcome to Your Vue.js App" />
        <SearchBar @termChange="onTermChange" />
    </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import SearchBar from "./components/SearchBar.vue";

export default {
    name: "App",
    components: {
        HelloWorld,
        SearchBar
    },
    methods: {
        onTermChange(searchTerm) {
            console.log(`parent: ${searchTerm}`);
        }
    }
};
</script>

<style>
#app {
    /* font-family: Avenir, Helvetica, Arial, sans-serif; */
    /* -webkit-font-smoothing: antialiased; */
    /* -moz-osx-font-smoothing: grayscale; */
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
