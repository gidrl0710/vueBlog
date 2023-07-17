<template>
  <div class="divTop">
    <div>
      <h5><router-link to='/detail/0' class="nav-link active">{{ dataList[0].title }}</router-link></h5>
      <!-- <h5 @click="$router.push('/detail/0')" class="nav-link active">{{ dataList[0].title }}</h5> -->
      <p>{{ dataList[0].date }}</p>
    </div>
    <div>
      <h5><router-link to='/detail/1' class="nav-link active">{{ dataList[1].title }}</router-link></h5>
      <p>{{ dataList[1].date }}</p>
    </div>
    <div>
      <h5><router-link to='/detail/2' class="nav-link active">{{ dataList[2].title }}</router-link></h5>
      <p>{{ dataList[2].date }}</p>
    </div>
    <div>
      <a class="nav-link" href="https://www.naver.com/">Naver</a> <a class="nav-link" href="https://www.google.com/">Google</a>
    </div>
  </div>
</template>

<script>

export default {
  name: 'TheList',
  props: {
    dataList: Array
  }

}
</script>

<style scoped>
div.divTop {
  margin-top: 50px;
}
</style>