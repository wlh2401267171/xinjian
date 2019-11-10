<template>
<div  id="top">
<div  class="top_head">
   <span>信件签收</span>
   <img src="@/assets/logo.png"/>
</div>
<hr/>
<div class="top_select">
    <input placeholder="搜索经办人.主办部室"/>
</div>


</div>
</template>
<script>
export default{
 methods:{}
}

</script>

<style lang="less">
#top{
    background-color: #f2f2f2;
    height: 1.8rem;
    .top_head{
        margin:0 0;
        // padding-top: 0.6rem;
        position: relative;
        span{
        display: block;
        font-size:0.48rem;
        color:black;
        text-align: center;
        }
        img{
            position: absolute;
            top:0;
            right:0.2rem;
            width: 0.5rem;
            height: 0.5rem;
        }
    }
    .top_select{
        margin-top:-0.7rem;
        input{
            border: none;
            // background-image: url();
            // background: no-repeat;
            outline: none;
            line-height: 0.8rem;
            border-radius: 0.2rem;
            font-size: 0.48rem;
            width:100%;
            // margin-bottom: 0.2rem;
        }
    }

}
</style>