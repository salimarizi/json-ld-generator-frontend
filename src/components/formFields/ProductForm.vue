<template>
  <div class="hello">
    <BrandForm item="item"/>
    <div class="row">
      <div class="col-md-3">
        <label for="">Product ID</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="product_id" placeholder="Product ID">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Name</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="name" placeholder="Name">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Image</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="image" placeholder="Image">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Description</label>
      </div>
      <div class="col-md-9">
        <textarea name="description" class="form-control" rows="4" placeholder="Description"></textarea>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">URL</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="url" placeholder="URL">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Audience Type</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="audience_type" placeholder="Audience Type">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Use Review</label>
      </div>
      <div class="col-md-2">
        <input type="checkbox" data-toggle="switchbutton" v-model="product_review">
      </div>
    </div>
    <hr>
    <div class="row" v-if="product_review">
      <div class="col-md-12">
        <h4>Review</h4>
      </div>
    </div>
    <ReviewForm item="product" v-if="product_review"/>
    <hr>
    <OfferForm/>
  </div>
</template>

<script>
import BrandForm from './BrandForm.vue'
import ReviewForm from './ReviewForm.vue'
import OfferForm from './OfferForm'

export default {
  name: 'ProductForm',
  components: {
    BrandForm,
    ReviewForm,
    OfferForm
  },
  data() {
    return {
      product_review: false
    }
  }
}
</script>
