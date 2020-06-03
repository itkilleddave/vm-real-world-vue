<template>
    <div id="nav">
        <nav>
            <router-link :to="{ name: 'event-list'}">List</router-link> |
            <router-link :to="{ name: 'event-create'}">Create</router-link> |
            <router-link :to="{ name: 'user', params: { username: 'Dave'} }">Dave</router-link> 
        </nav>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>

</style>