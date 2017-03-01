<template>
  <div>
    <span class="title">欢迎登录</span>
    <divider>Vue Vux</divider>
    <Group>
      <XInput title="账号" v-module='account' placeholder='账号' type='text'></XInput> 
      
    </Group>
    <X-input title="密码" v-module='password' placeholder='密码' type="password"></X-input>
    <XButton type="primary" action-type="button">登录</XButton>
  </div>
</template>

<script>
  import { Divider, Group, XInput, XButton } from 'vux'
  export default {
    components: {
      Divider,
      Group,
      XInput,
      XButton
    },
    data () {
      return {
        account: '',
        password: ''
      }
    }
  }
</script>
