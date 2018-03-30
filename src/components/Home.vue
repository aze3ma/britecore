<template>
  <div>
    <Header />
    <MainCard />
  </div>
</template>

<script>
import Header from './Header'
import MainCard from './MainCard'

export default {
  name: 'Home',
  components: {
    Header,
    MainCard
  }
}
</script>
