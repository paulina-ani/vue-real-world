<template>
    <div>
        <h1>Event list</h1>

        <router-link :to="{ name: 'event-show', params: { id: '1'} }">Show event</router-link>
    </div>
</template>

<script>
    export default {
        name: "EventList"
    }
</script>

<style scoped>

</style>