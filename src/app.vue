<template>
    <div class="example">
        {{msg}}
        <span>less-123</span>
    </div>
</template>

<script>
    export default{
        data(){
            return{
                msg: 'hello! webpack4-vue-demo!'
            }
        }
    }
</script>

<style lang='less'>
    .example {
        color: red;
        span{
            color:blue;
        }
    }
</style>
