<template>
  <h1>Hello from Nuxt! This is {{which}}-side rendered.</h1>
</template>
</<script>
export default {
  asyncData ({ isStatic, isServer }) {
    return {
      which: isStatic ? 'static' : (isServer ? 'server' : 'client')
    }
  }
}
</script>
