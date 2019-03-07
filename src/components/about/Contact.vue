<template>
    <div class="contact">
        <!-- <h1>这是contact的页面</h1> -->
        <div class="card text-center">
            <div class="card-header">
                Featured
            </div>
            <div class="card-body">
                <h5 class="card-title text-dark">联系我们</h5>
                <p class="card-text text-danger">欢迎来道炫酷世界,大家嗨起来</p>
                <router-link to="/contact/address" class="btn btn-primary">地址信息</router-link>
                <router-link to="/contact/person" class="btn btn-primary">法人代表</router-link>
                <router-link to="/contact/tel" class="btn btn-primary">投诉电话</router-link>
                <router-view></router-view>
            </div>
            <div class="card-footer text-muted" id="box1">
                2 days ago
            </div>
        </div>
    </div>
</template>

<script>
// 获取时间
// var box1 = document.getElementById('box1');
// var date = new Date();
// console.log(data);
// var hour = date.getHours(); // 小时
// var min = date.getMinutes(); // 分钟
// var sec = date.getSeconds(); // 秒
// box1.innerHTML =hour+ ':' + min + ':' + sec ;
export default {
    name:'Contact',
    data(){
        return{

        }
    }
}
</script>

<style scoped>

</style>