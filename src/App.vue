<template>
    <div class="container cd">
        <p>Count: <strong class="font-italic">{{ count }}</strong></p>
        <button class="btn btn-danger" v-on:click="increment">Increment</button>
        <button class="btn btn-warning" v-on:click="dicrement">Dicrement</button>
    </div>
</template>
<script>
export default {
    data(){
        return{
            count: 0,
        }
    },
    methods: {
        increment(){
            this.count += 1
        },
        dicrement(){
            this.count -= 1
        }
    },
}
</script>
<style>
.cd{
    display: flex;
    flex-direction: column;
    align-content: center;
    justify-content: center;
    align-items: center;
    padding-top: 100px;
    font-size: 50px;
}
button{
    border-radius: 20px !important;
    border: 2px solid coral !important;
    padding: 10px !important;
    font-size: 20px !important;
    width: 200px;
    margin-top: 10px;
    margin-bottom: 10px;
}
</style>