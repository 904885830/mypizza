<template>
    <div class="activity">
        <!-- <h1>这是activity的页面</h1> -->
        <div class="card col-12 mb-5" v-for="(item,index) in items" :key="index">
        <img class="card-img-top " src="../../assets/timg.jpg" alt="Card image cap">
            <div class="card-body">
                <h5 class="card-title">{{item.title}}</h5>
                <p class="card-text">{{item.text}}</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'Activity',
    data(){
        return{
            items:[
                {title:'热门活动1',text:'三八女王节,有机会抽中免单!!!'},
                {title:'热门活动2',text:'三八女王节,有机会抽中免单!!!'},
                {title:'热门活动3',text:'三八女王节,有机会抽中免单!!!'}
            ]
        }
    }
}
</script>

<style scoped>

</style>