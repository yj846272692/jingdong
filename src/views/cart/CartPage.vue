<template>
    <div>
        <h2>购物车</h2>
        <AppDocker :currentIndex="1" />
    </div>
</template>
<script>
import AppDocker from '../../components/AppDocker'
export default {
  name: 'CarPage',
  components: {
    AppDocker
  }
}
</script>
<style lang="scss" scoped>

</style>
