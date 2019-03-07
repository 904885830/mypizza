<template>
    <div class="delivery row">
        <!-- <h1>这是delivery的页面</h1> -->
        <div class="card col-4" v-for="(item,index) in items" :key="index">
            <img class="card-img-top" :src="item.imgSrc" alt="Card image cap">
            <div class="card-body">
                <h4 class="card-title">{{item.title}}</h4>
                <p class="card-text text-success">{{item.text}}</p>
                <button @click="alert1">快递查询</button>
            </div>
        </div>
    </div>
</template>

<script>
// 图片是静态资源,需要单独引入
// 第一种方法
// import sf from '../.../assets/del-sf.png'
export default {
    name:'Delivery',
    data(){
        return{
            items:[
                {imgSrc:require('../../assets/del-sf.png'),title:'顺风速运',text:'您的快递信息已发送至澳大利亚'},
                {imgSrc:require('../../assets/del-yt.jpg'),title:'圆通快递',text:'您的快递信息已发送至马尔代夫'},
                {imgSrc:require('../../assets/del-zt.jpg'),title:'中通快递',text:'您的快递信息已发送至爱琴海'}
            ]
        }
    },
    methods:{
        alert1(){
            alert('当前快递小姐姐正在快马加鞭为您派送!!!')
        }
    }
}
</script>

<style scoped>
img{
    width: 100%;
    height: 50%;
}
</style>