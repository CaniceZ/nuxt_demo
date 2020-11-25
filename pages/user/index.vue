<template>
    <div>
      {{project}}
    </div>
</template>

<script>
  export default {
    head: {
      title: 'user page'
    },
    data() {
      return { project: 'user' }
    },
    asyncData(context) {
      return { project: 'user2' }
    }
  }
</script>

<style scoped>

</style>
