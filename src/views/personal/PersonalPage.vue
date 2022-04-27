<template>
    <div>
        <h2>我的</h2>
        <router-link to="login">
          <h2>登录</h2>
        </router-link>
        <AppDocker :currentIndex="3" />
    </div>
</template>
<script>
import AppDocker from '../../components/AppDocker'
export default {
  name: 'PersonalPage',
  components: {
    AppDocker
  }
}
</script>
<style lang="scss" scoped>

</style>
