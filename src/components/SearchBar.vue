<template>
    <div><input @input="onInput" /></div>
</template>

<script>
export default {
    name: "SearchBar",
    methods: {
        onInput(event) {
            /* console.log(`value: ${event.target.value}`); */
            this.$emit("termChange", event.target.value);
        }
    }
};
</script>
<style></style>
