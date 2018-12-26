<template>
  <div class="m-menu">
    <dl class="nav">
      <dt>全部分类</dt>
      <dd
        v-for="(item,idx) in listMenu"
        :key="idx"
      >
        <i :class="item.type"/>{{ item.name }}<span class="arrow"/>
      </dd>
    </dl>
    <div
      v-if="false"
      class="detail"
    >
      <!--<template v-for="(item,idx) in curdetail.child">
        <h4 :key="idx">{{ item.title }}</h4>
        <span
          v-for="v in item.child"
          :key="v">{{ v }}</span>
      </template>-->
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        listMenu: [{type: 'food',name: '美食'}, {type: 'takeout', name: '外卖'}]
      }
    },
    methods: {
      enter() {
      }
    }
  }
</script>

<style scoped>

</style>
