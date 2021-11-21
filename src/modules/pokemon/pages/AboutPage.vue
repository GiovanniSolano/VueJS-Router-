<template>
    <h1>About Page</h1>
    <hr>
    <!-- <h2>{{name}}</h2> -->
    <button @click="onChangeName">
        Cambiar nombre
    </button>
</template>

<script>
export default {

    data() {
        return {
            name: 'Giovanni'
        }
    },
    methods: {
        onChangeName(){
            console.log('Se cambiara el nombre');
            this.name = 'Solano'
            // PETICIONES HTTP
        }
    },

    beforeCreate() {
        console.log('beforeCreate');
    },
    created() {
        console.log('created');
    },
    beforeMount() {
        console.log('beforeMount');
    },
    beforeUnmount() {
        console.log('beforeUnmount');
    },
    mounted() {
        console.log('mounted');
    },
    beforeUpdate() {
        console.log('beforeUpdate');
    },
    updated() {
        console.log('updated');
    },
    activated() {
        console.log('activated');
    },
    deactivated() {
        console.log('deactivated');
    },
    unmounted() {
        console.log('unmounted');
    },
    errorCaptured() {
        console.log('errorCaptured');
    },
    renderTracked() {
        console.log('renderTracked');
    },
    renderTriggered() {
        console.log('renderTriggered');
    },
}
</script>