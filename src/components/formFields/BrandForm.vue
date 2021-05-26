<template>
  <div class="hello">
    <div class="row">
      <div class="col-md-3">
        <label for="">Brand Logo</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="brand_logo" placeholder="Brand Logo">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Brand Slogan</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="brand_slogan" placeholder="Brand Slogan">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Brand Description</label>
      </div>
      <div class="col-md-9">
        <textarea name="brand_description" class="form-control" rows="4" placeholder="Brand Description"></textarea>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Brand Alternate Name</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="brand_alternate_name" placeholder="Brand Alternate Name">
      </div>
    </div>
    <div class="row" v-if="!item">
      <div class="col-md-3">
        <label for="">Use Rating</label>
      </div>
      <div class="col-md-2">
        <input type="checkbox" data-toggle="switchbutton" v-model="brand_rating">
      </div>
    </div>
    <hr>
    <RatingForm isAggregate="true" v-if="brand_rating"/>
  </div>
</template>

<script>
import RatingForm from './RatingForm.vue'
export default {
  name: 'BrandForm',
  components: {
    RatingForm
  },
  props: {
    item: String
  },
  data() {
    return {
      brand_rating: false
    }
  }
}
</script>
