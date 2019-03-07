<template>
    <div class="telphone">
        <!-- <h1>这是telphone的页面</h1> -->
        <h3 class="mt-3">欢迎拨打: {{tel}}</h3>
    </div>
</template>

<script>
export default {
    name:'Telphone',
    data(){
        return{
            tel:'119-120-110'
        }
    }
}
</script>



<style scoped>

</style>
