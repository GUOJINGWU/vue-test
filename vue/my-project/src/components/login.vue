// login.vue
<template>
  <div>
      <h2>Login</h2>
      <hr/>
      <p>{{content}}</p>
      <input  v-model="Username">
      <p>您输入的用户名为：{{ Username }}</p>
       <input  v-model="Password">
      <p>您输入的密码为：{{ Password }}</p>
      <button type="submit" v-on:click="login">登录</button>





      <div style="width:168px;margin:0 auto">
        <ol>
          <li v-for="todo in todos">
            {{ todo.text }}
          </li>
        </ol>
      </div>

      <div>
        <p>{{ message }}</p>
        <button v-on:click="reverseMessage">逆转消息</button>
      </div>



  </div>
  
</template>
<script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
<script>

export default {
  data() {
    return {
      content: "this is Login components",
      Username:"Ryan",
      Password:123456,
      message: "Hello,vue.js!",

      todos: [
      { text: '学习 JavaScript' },
      { text: '学习 Vue' },
      { text: '整个牛项目' }
    ]


    }
  },
  methods:{
    login:function(){
      alert(2)
    },
     reverseMessage: function () {
      this.message = this.message.split('').reverse().join('')
    }
  }
 
};
</script>

