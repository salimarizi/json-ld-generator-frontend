<template>
  <div class="hello">
    <div v-if="!item">
      <div class="row">
        <div class="col-md-3">
          <label for="">Item Reviewed Name</label>
        </div>
        <div class="col-md-9">
          <input type="text" class="form-control" name="item_name" placeholder="Name">
        </div>
      </div>
      <div class="row">
        <div class="col-md-3">
          <label for="">Item Reviewed URL</label>
        </div>
        <div class="col-md-9">
          <input type="text" class="form-control" name="item_url" placeholder="URL">
        </div>
      </div>
      <div class="row">
        <div class="col-md-3">
          <label for="">Item Reviewed Description</label>
        </div>
        <div class="col-md-9">
          <textarea name="item_description" class="form-control" rows="4" placeholder="Description"></textarea>
        </div>
      </div>
    </div>

    <RatingForm isAggregate="false"/>
    
    <div class="row">
      <div class="col-md-3">
        <label for="">About</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="about" placeholder="About">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Review Aspect</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="review_aspect" placeholder="Review Aspect">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Review Body</label>
      </div>
      <div class="col-md-9">
        <textarea name="review_body" class="form-control" rows="4" placeholder="Review Body"></textarea>
      </div>
    </div>
    <hr>
    <div class="row">
      <div class="col-md-12">
        <h4>Person Reviewed</h4>
      </div>
    </div>
    <AuthorForm/>
  </div>
</template>

<script>
import AuthorForm from './AuthorForm.vue'
import RatingForm from './RatingForm.vue'

export default {
  name: 'ReviewForm',
  props: {
    item: String
  },
  components: {
    AuthorForm,
    RatingForm
  }
}
</script>
