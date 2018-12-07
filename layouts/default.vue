<template>
  <el-container class="layout-default">
    <el-header>
      <myHeader/>
    </el-header>
    <el-main>
      <div>
        <nuxt/>
      </div>
    </el-main>
    <el-footer>Footer</el-footer>
  </el-container>
</template>

<script>
  import myHeader from '@/components/public/header/index'
  export default {
    components: {
      myHeader
    }
  }
</script>

<style lang="scss">

</style>
