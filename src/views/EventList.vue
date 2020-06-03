<template>
    <div>
        <h1>Event Listings</h1>
        <event-card/>
        <base-icon/>
    </div>
</template>

<script>

import EventCard from '../components/EventCard.vue'

export default {
    components: {
        EventCard
    }
}
</script>