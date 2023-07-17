<template>
  <div class="divTop">
    <!-- {{ dataList[$route.params.id].number }} -->
    <h3>상세 페이지</h3>
    <h5>{{ dataList[$route.params.id].title }}</h5>
    <p>{{ dataList[$route.params.id].content }}</p>
    <p>{{ dataList[$route.params.id].date }}</p>
  </div>
</template>

<script>
export default {
  name: 'TheDetail',
  props: {
    dataList: Array
  }
}
</script>

<style>
div.divTop {
  margin-top: 50px;
}
</style>