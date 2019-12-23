<template>
    <div>
        <h4> {{ title }}</h4>
    </div>
</template>

<script>
    export default {
        name: "EventCard",
        data() {
            return {
                event: {
                    id: 1,
                    title: "Beach Cleanup",
                    date: "Tues Aug 19, 2018",
                    time: "06.00",
                    attendees: [
                        { id: "abc123", name: "Paulina Ani" },
                        { id: "def456", name: "John Doe"}
                    ]
                }
            }
        }
    }
</script>

<style scoped>
    .event-card {
        padding: 20px;
        margin-bottom: 24px;
        transition: all 0.2s linear;
        cursor: pointer;
    }
    .event-card:hover {
        transform: scale(1.01);
        box-shadow: 0 3px 12px 0 rgba(0, 0, 0, 0.2), 0 1px 15px 0 rgba(0, 0, 0, 0.19);
    }
    .event-card > .title {
        margin: 0;
    }

    .event-link {
        color: black;
        text-decoration: none;
        font-weight: 100;
    }
</style>