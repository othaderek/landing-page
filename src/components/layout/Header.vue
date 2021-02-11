<template>
    <header class="header">
        <p>odhp</p>
        <img src="@/assets/pic.png" alt="" id="image">
    </header>
</template>

<script>
export default {
    name: "Header"
}
</script>

<style scoped>
    .header{
        color: white;
        justify-content: center;
        text-align: center;
    }
    #image{
        justify-content: center;
        height: auto; 
        width: auto; 
        max-width: 150px; 
        max-height: 150px;
        margin-bottom: 15px;
        border-radius: 50%;
    }
</style>