<template>
    <div>
      <h3>userDetails 异步数据</h3>
      <div>apiUrl： {{urls.apiUrl}}</div>
      <div>apilogUrl： {{urls.apilogUrl}}</div>
      <div>h5csUrl： {{urls.h5csUrl}}</div>
    </div>
</template>

<script>
  import axios from 'axios'
  export default {
    head: {
      title: 'userDetails page'
    },
    async asyncData ({ params }) {
      let { data } = await axios({
        method: 'get',
        url: 'http://test-h5sdk.917youxi.com/Api/getHDomain.do'
      })
      return { urls: data }
    },
  }
</script>

<style scoped>

</style>
