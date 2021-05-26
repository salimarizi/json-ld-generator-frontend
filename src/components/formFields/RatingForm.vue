<template>
  <div class="hello">
    <div class="row">
      <div class="col-md-12">
        <h4>Rating</h4>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Rating Value</label>
      </div>
      <div class="col-md-4">
        <input type="number" class="form-control" name="rating_value" placeholder="Rating Value">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Best Rating Value</label>
      </div>
      <div class="col-md-4">
        <input type="number" class="form-control" name="best_rating" placeholder="Rating Value">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Worst Rating Value</label>
      </div>
      <div class="col-md-4">
        <input type="number" class="form-control" name="worst_rating" placeholder="Rating Value">
      </div>
    </div>
    <div class="row" v-if="isAggregate == true">
      <div class="col-md-3">
        <label for="">Rating Count</label>
      </div>
      <div class="col-md-4">
        <input type="number" class="form-control" name="rating_count" placeholder="Rating Value">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Explanation</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="explanation" placeholder="Explanation">
      </div>
    </div>
    <hr>
  </div>
</template>

<script>
export default {
  name: 'RatingForm',
  props: {
    isAggregate: Boolean
  }
}
</script>
