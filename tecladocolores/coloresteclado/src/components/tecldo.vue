<template >
    <div id="root">
        <h1>Mi primer componente</h1>
        Presione una tecla
        <input type="text" v-on:keydown="key">
        Tecla presionada: {{keycode}}
    </div>
</template>
<script>
export default {
    name:'tecladocolor',
    data(){
        return{
            title: "cololes de teclas",
            keycode: ''
        }
    },
    methods:{
        key(event){
            this.keycode = event.keyCode
        }
    }
}
</script>