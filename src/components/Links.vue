<template>
<div>
    <div v-for="link in linkItems" v-bind:key="link.id" class="container">
        <LinkItem v-bind:link="link"/>
    </div>
</div>
</template>

<script>
import LinkItem from './LinkItem'
export default {
    name: "Links",
    components: {LinkItem},
    data(){
        return {
            linkItems: [
                
                {
                    id: 1,
                    title: "Spotify",
                    link: "https://distrokid.com/hyperfollow/othaderekhernandezpena/our-june"
                },
                {
                    id: 2,
                    title: "Youtube",
                    link: "https://youtu.be/FDUKjMiDIuc"
                },
                {
                    id: 3,
                    title: "Instagram",
                    link: "https://www.instagram.com/_odhp_"
                }
            ]
        }
    }
}
</script>

<style scoped>

</style>