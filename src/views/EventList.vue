<template>
    <div>
        <h1>Event list</h1>
        <EventCard></EventCard>
    </div>
</template>

<script>
    import EventCard from "../components/EventCard";
    import axios from "axios";
    export default {
        name: "EventList",
        components: {
            EventCard
        },
        created() {
            axios
                .get('http://localhost:3000/events')
                .then(response => {
                    console.log(response.data)
                })
                .catch(error => {
                    console.log("There was an error:" + error.response)
                })
        }
    }
</script>

<style scoped>

</style>