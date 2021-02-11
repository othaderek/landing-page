<template>
    <div class="link" @click="handleClick">
        <p class="text">{{link.title}}</p>
    </div>
</template>

<script>
export default {
    name: "LinkItem",
    props:["link"],
    methods: {
        handleClick(){
            window.open(this.link.link, "_blank")
        }
    }
    
}
</script>

<style scoped>

</style>