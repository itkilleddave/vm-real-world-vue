<template>
    <router-link class="event-link" :to="{ name: 'event-show', params: {id: 1}}">
        <div class="event-card -shadow">
            <span class="eyebrow">@{{event.time}} on {{event.date}}</span>
            <h4 class="title">{{ event.title }}</h4>
            <base-icon name="users">
                <h3 slot="pre-icon">Slotto!</h3>
                <span slot="post-icon">{{ event.attendees.length }} attending</span>
                <template slot="my-template">
                    <h4>Some Template Heading</h4>
                    <base-icon name="award"/>
                </template>
            </base-icon>
        </div>
    </router-link>
</template>

<script>
export default {
    data() {
        return {
            event: {
                id: 1,
                title: 'Beach Cleanup',
                date: 'Tue May 15 2018',
                time: '6:00',
                attendees: [
                { id: 'abc123', name: 'Adam Jahr' },
                { id: 'def456', name: 'Gregg Pollack' }
                ]
            }
        }
    }
}
</script>

<style scoped>
h4 {
    color: green;
}
</style>