<template>
    <div>
        <h1>Event list</h1>
        <EventCard></EventCard>
        <router-link :to="{ name: 'event-show', params: { id: '1'} }">Show event</router-link>
    </div>
</template>

<script>
    import EventCard from "../components/EventCard";
    export default {
        name: "EventList",
        components: {
            EventCard
        }
    }
</script>

<style scoped>

</style>