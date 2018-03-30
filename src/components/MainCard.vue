<template>
  <section class="main-card container">
    <h2 class="main-card__header">{{ header }}</h2>
    <div class="row row--4">
      <FieldTypes class="col" />
      <FieldDetails class="col col-three-fourths" />
    </div>
    <Footer />
  </section>
</template>

<script>
import FieldTypes from './FieldTypes'
import FieldDetails from './FieldDetails'
import Footer from './Footer'

export default {
  name: 'MainCard',
  components: {
    FieldTypes,
    FieldDetails,
    Footer
  },
  data () {
    return {
      header: 'Commercial Property - Add Field'
    }
  }
}
</script>
