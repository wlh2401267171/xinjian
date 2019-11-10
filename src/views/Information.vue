<template>
    <div id="inf">
        <div class="inf_top">
            <span @click="fanhui">返回</span>
            <div>详细信息</div>
        </div>
        <div class="inf_content">
            <div><span>主办部室：</span> <strong>党委办公室</strong></div>
            <div><span>日期：</span> <strong>2019-09-23</strong></div>
            <div><span>经办人：</span> <strong>王炼辉</strong></div>
            <div><span>联系电话：</span> <strong>123456</strong></div>
            <div><span>信件类型：</span> <strong>交换文件</strong></div>
            <div><span>发往单位：</span> <strong>财政部</strong></div>
            <div><span>寄送点：</span> <strong>室内</strong></div>
            <div><span>详细地址：</span> <strong>xx省xx州xx路</strong></div>
            <div><span>内容：</span> <strong>xxxxxx</strong></div>
            <div><button>提交</button></div>
        </div>

    </div>
</template>
<script>
export default {
    methods:{
        fanhui:function(){
            this.$router.push({
                path: '/about'
            })
        }
    }
    
}
</script>

<style lang="less">
#inf{
    font-size:0.38rem;
    line-height: 0.72rem;
    .inf_top{
        margin-top:0.5rem;
        display: flex;
        span{
            color: red;
        }
        div{
            width: 74%;
            text-align: center;
           
        }

    }
}


</style>