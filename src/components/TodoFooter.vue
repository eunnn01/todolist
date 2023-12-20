<template>
    <div class="ClearAllContainer">
        <span class="ClearAllBtn" @click="clearTodo">Clear All</span>
    </div>
</template>
<script>
export default{
    methods: {
        clearTodo(){
            this.$emit('removeAll');
        }
    }
}
</script>

<style>
    .ClearAllContainer{
        width: 8.5rem;
        height: 50px;
        line-height: 50px;
        background-color: white;
        border-radius: 5px;
        margin: 0 auto;
        margin-top: 20px;
    }
    .ClearAllBtn{
        color: #e20303;
        display: block;
    }
</style>