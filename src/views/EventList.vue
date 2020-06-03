<template>
    <div>
        <h1>Event Listings</h1>
        <event-card/>
        <base-icon name="award" width="50" height="50"/>
        <base-icon name="battery" width="50" height="50"/>
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