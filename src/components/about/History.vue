<template>
    <div class="history row ">
        <!-- <h1>这是history的页面</h1> -->
        <div class="card col-4" v-for="(item,index) in items" :key="index">
            <img class="card-img-top" :src="item.imgsrc" alt="Card image cap">
            <div class="card-body">
                <h4 class="card-title">{{item.title}}*{{item.num}}</h4>
                <p class="card-text text-success">{{item.text}}</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'History',
    data(){
        return{
            items:[
                {imgsrc:require('../../assets/mao.jpg'),title:'猫仔',num:4,text:'已完成支付'},
                {imgsrc:require('../../assets/timg.jpg'),title:'海豹',num:2,text:'已完成支付'},
                {imgsrc:require('../../assets/yue.jpeg'),title:'月狮',num:3,text:'已完成支付'}
            ],
        }
    }
}
</script>

<style scoped>
img{
    width: 100%;
    height: 200px;
}
</style>

