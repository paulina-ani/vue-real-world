<template>
    <h1>This is a page for {{ username }}</h1>
</template>

<script>
    export default {
        name: "User",
        props: ["username"]
    }
</script>

<style scoped>

</style>