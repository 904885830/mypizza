<template>
<div class="admin">
    <!-- <h1>这是admin的页面</h1>  -->
    <div class="col-7">
        <NewPizza></NewPizza>
    </div>
    <div class="col-5"></div>
</div>
</template>

<script>
import NewPizza from '@/components/NewPizza'
export default {
    name: 'Admin',
    data () {
        return {
        
        }
    },
    components:{
        'NewPizza': NewPizza
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
