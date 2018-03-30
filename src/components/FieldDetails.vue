<template>
  <section class="field-details">
    <h3 class="field-details__header">Field Details</h3>
    <form class="field-details__form">
      <div class="wrapper">
        <div class="field-details__field">
          <label for="label">Display Label</label>
          <input type="text" name="label" id="label" autocomplete="off" />
          <span class="minor-message">For display purposes, spaces allowed</span>
        </div>
        <div class="field-details__field">
          <label for="reference">Reference Name</label>
          <input type="text" name="reference" id="reference" autocomplete="off" />
          <span class="minor-message">Used to reference in calculations, no spaces allowed</span>
        </div>
      </div>
      <div class="field-details__field">
        <label for="default">Default Value</label>
        <input type="text" name="label" id="label" autocomplete="off" />
      </div>
      <div class="field-details__field">
        <label for="validation">Custom Validation</label>
        <input type="text" name="validation" id="label" autocomplete="off" />
        <span class="minor-message">Any regex pattern can be used for custom input validation</span>
      </div>
      <h4>Tags</h4>
      <p>Tag Group</p>
      <div class="wrapper wrapper--tags">
        <div class="field-details__field">
          <label for="vinmaster">Vinmaster</label>
          <input type="checkbox" name="vinmaster" id="vinmaster" />
        </div>
        <div class="field-details__field">
          <label for="iso">ISO</label>
          <input type="checkbox" name="iso" id="iso" />
        </div>
        <div class="field-details__field">
          <label for="tag">Tag 3</label>
          <input type="checkbox" name="tag" id="tag" />
        </div>
      </div>
      <h4>Tags</h4>
      <div class="tags-result">
        <p>Select a tag group to see individual groups</p>
      </div>
    </form>
    <aside class="field-details__groups-list">
      <h4>Field Groups</h4>
      <p>Choos a group for this input</p>
      <div class="field-details__groups-item">
        <h5>Rental Vehicle Coverage Package</h5>
        <p>7 other inputs</p>
      </div>
    </aside>
  </section>
</template>

<script>
export default {
  name: 'FieldDetails'
}
</script>
