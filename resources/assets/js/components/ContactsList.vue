<template>
    <div class="contact-list">
        <ul>
            <li v-for="contact in contacts"
                :key="contact.id"
            >
                <div class="avatar">
                    <img :src="contact.profile_image" :alt="contact.name">
                </div>
                <div class="contact">
                    <div class="name">{{contact.name}}</div>
                    <div class="email">{{contact.email}}</div>
                </div>

            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        name: "ContactsList",
        props: {
            contacts: {
                type: Array,
                default: []
            }
        }
    }
</script>

<style scoped>

</style>