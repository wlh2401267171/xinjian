<template>
  <div id="home">
    <ul>
      <li v-for="(item,index) in message" :key="index">
       <div><span class="about_span">经办人:</span><span v-text="item.title"></span></div> 
       <div><span class="about_span">主办单位:</span><span v-text="item.location"></span></div>
       <div><span class="about_span">发往单位:</span><span v-text="item.to"></span><br/></div>
       <div class="about_foot"><strong>签收</strong> <strong>退回</strong> </div>
    
      </li>
    </ul>
  </div>

</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'


export default {
  name: 'home',
  components: {
    HelloWorld,
  },
  data(){
    return{
    message:[
      {title:"王先生",location:"法律事务部(消费者权益办公室)",to:"中国工商银行(上海分行)"},
      {title:"李先生",location:"法律事务部(消费者权益办公室)",to:"中国工商银行(上海分行)"},
      {title:"经办人:高先生",location:"法律事务部(消费者权益办公室)",to:"中国工商银行(上海分行)"},
    ]
    }
    }
  
}
</script>
<style lang="less">

#home{
  ul{
    li{
      font-size: 0.35rem;
      margin:0.25rem auto;
      list-style: none;
      line-height: 0.85rem;
      .about_span{
        font-size: 0.35rem;
        color: gray;
        font-weight: 100;
      }
      .about_foot{
        display: flex;
        strong{
          flex-direction: column;
          width: 50%;
          color: blue;
        }
      }
    }
  }
}


</style>