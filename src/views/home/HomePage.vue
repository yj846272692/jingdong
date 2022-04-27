<template>
    <div class="wrapper">
        <StaticPart />
        <NearbyShop />
    </div>
    <AppDocker :currentIndex="0" />
</template>
<script>
import StaticPart from './StaticPart'
import NearbyShop from './NearbyShop'
import AppDocker from '../../components/AppDocker'
export default {
  name: 'HomePage',
  components: { StaticPart, NearbyShop, AppDocker }
}
</script>
<style lang="scss" scoped>
    .wrapper {
        overflow-y: auto;
        position: absolute;
        left: 0;
        top: 0;
        bottom: 0.5rem;
        right: 0;
        padding: 0 0.18rem 0.1rem 0.18rem;
    }
</style>
