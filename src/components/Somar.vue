<template>
    <button class="btn">{{text}}</button>
</template>

<script>
    export default {
        name: 'OlhaSo',
        data(){
            return {
                text: 'Clique Aqui'
            }
        }
        
    }
</script>

<style lang="scss">
    .btn {
        padding: 20px 10px;
        background-color: white;
        border: 1px solid black;
        margin-top: 10px;
        cursor: pointer;
        border-radius: 2px;
        box-sizing: border-box;
        transition: 0.2s;

        &:hover {
            background-color: black;
            color: white;
            border: 1px solid white;
        }
    }
</style>