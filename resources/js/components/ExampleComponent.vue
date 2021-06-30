<template>
   
</template>

<script>
    export default {
        mounted() {
            Echo.channel('test')
                .listen('Test', (e)=>{
                    console.log(e);
                });
            console.log('Component mounted.')
        }
    }
</script>


// hello