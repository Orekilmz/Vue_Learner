<script>
//声明式渲染,提高开发效率
export default{
    data(){
      return{
        num:0,
        uname:"Jack",
        msg:"<h2>my first vue page</h2>"
      }
    },
    methods:{//vue定义方法
      UnameChange:function(){
        this.uname="张三"
      },
      helloworld:function(){
        alert('helloworld!')
      }
    },
}
</script>

<template>
<ul>
  home
</ul>
<p>这是个指向
  <a href="https://www.baidu.com" title="尝试百度跳转">百度
  </a>
  的链接</p>

<p>working together…</p>

  <p v-html="msg"></p>
  <p>{{num}}</p>
  <p>uname</p>
  <p v-once>{{ uname }}</p>
  <p>{{ uname }}</p>
  <button @click="UnameChange">改变名字</button>
  <button @click="helloworld">你好</button>
  <ol>
  <li>
    先用蛋白一个、盐半茶匙及淀粉两大匙搅拌均匀，调成“腌料”，鸡胸肉切成约一厘米见方的碎丁并用“腌料”搅拌均匀，腌渍半小时。
  </li>
  <li>
    用酱油一大匙、淀粉水一大匙、糖半茶匙、盐四分之一茶匙、白醋一茶匙、蒜末半茶匙调拌均匀，调成“综合调味料”。
  </li>
  <li>
    鸡丁腌好以后，色拉油下锅烧热，先将鸡丁倒入锅内，用大火快炸半分钟，炸到变色之后，捞出来沥干油汁备用。
  </li>
  <li>
    在锅里留下约两大匙油，烧热后将切好的干辣椒下锅，用小火炒香后，再放入花椒粒和葱段一起爆香。随后鸡丁重新下锅，用大火快炒片刻后，再倒入“综合调味料”继续快炒。
  </li>
  <li>如果你采用正宗川菜做法，最后只需加入花生米，炒拌几下就可以起锅了。</li>
  <li>如果你在北方，可加入黄瓜丁、胡萝卜丁和花生米，翻炒后起锅。</li>
</ol>

<ol>
  <li>
    先用蛋白一个、盐半茶匙及淀粉两大匙搅拌均匀，调成“腌料”，鸡胸肉切成约一厘米见方的碎丁并用“腌料”搅拌均匀，腌渍半小时。
  </li>
  <li>
    用酱油一大匙、淀粉水一大匙、糖半茶匙、盐四分之一茶匙、白醋一茶匙、蒜末半茶匙调拌均匀，调成“综合调味料”。
  </li>
  <li>
    鸡丁腌好以后，色拉油下锅烧热，先将鸡丁倒入锅内，用大火快炸半分钟，炸到变色之后，捞出来沥干油汁备用。
  </li>
  <li>
    在锅里留下约两大匙油，烧热后将切好的干辣椒下锅，用小火炒香后，再放入花椒粒和葱段一起爆香。随后鸡丁重新下锅，用大火快炒片刻后，再倒入“综合调味料”继续快炒。
    <ul>
      <li>
        如果你采用正宗川菜做法，最后只需加入花生米，炒拌几下就可以起锅了。
      </li>
      <li>如果你在北方，可加入黄瓜丁、胡萝卜丁和花生米，翻炒后起锅。</li>
    </ul>
  </li>
</ol>
<ul>
  <li><a href="../index.html">home</a></li>
  <li><a href="../pictures.html">pictures</a></li>
  <li><a href="../projects.html">projects</a></li>
</ul>
</template>