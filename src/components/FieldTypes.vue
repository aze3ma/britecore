<template>
  <section class="field-types">
    <h3 class="field-types__header">{{ header }}</h3>
    <form class="field-types__filter-form">
      <label for="search">Filter Types</label>
      <input type="text" id="search" name="search" autocomplete="off" />
    </form>
    <ul class="field-types__cards-list list">
      <li class="field-types__cards-item" v-for="(fieldType, index) in fieldTypes" v-bind:key="fieldType.type"
          v-bind:class="[ isActive ? 'field-types__cards-item--active' : '' ]" @click="toggleCardState($event, index)">
        <dl>
          <div class="card-wrapper">
            <dt class="field-types__label" v-if="fieldType.type === 'Text'">H</dt>
            <dt class="field-types__label" v-else-if="fieldType.type === 'Date'"><i class="ion-android-calendar"></i></dt>
            <dt class="field-types__label" v-else><i class="ion-android-car"></i></dt>
            <dd class="field-types__value">{{ fieldType.type }}</dd>
          </div>
          <div class="card-wrapper">
            <dt class="field-types__label">Definition</dt>
            <dd class="field-types__value">{{ fieldType.definition }}</dd>
          </div>
          <div class="card-wrapper">
            <dt class="field-types__label">Default</dt>
            <dd class="field-types__value">{{ fieldType.default }}</dd>
          </div>
        </dl>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  name: 'FieldTypes',
  data () {
    return {
      isActive: false,
      header: 'Field Types',
      fieldTypes: [
        { type: 'Text', definition: 'String of text', default: 'Free-form text input' },
        { type: 'Date', definition: 'Standard ISO format date', default: 'Datepicker, with configurable format' },
        { type: 'VIN', definition: 'Vehichle Identification Number', default: 'Free-form text input' }
      ]
    }
  },
  methods: {
    toggleCardState (event, i) {
      this.isActive = !this.isActive
    }
  }
}
</script>
