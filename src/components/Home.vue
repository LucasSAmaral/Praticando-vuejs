<template>
    <div class="teste">
        <p>{{ola}}</p>
        {{numero}}
        <Somar @click.native="aumenta"></Somar>
    </div>
</template>

<script>
    import $ from 'jquery';
    import Somar from './Somar';
    export default {
        name: 'Home',
        data() {
            return {
                ola: 'SOMANDO...',
                numero: 0
            }
        },
        methods: {
            aumenta: function(){
                this.numero = this.numero + 1;
                
            },
        },
        components: {Somar}
    }
    
</script>

<style lang="scss">
    .teste {
        width: 200px;
        height: 200px;
        background-color: #000;
        margin: 0 auto;
        color: #fff;
        display: flex;
        flex-direction: column;
        justify-content: center;
        box-sizing: border-box;
        padding: 10px;
        font-weight: bold;
    }
</style>