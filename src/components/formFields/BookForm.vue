<template>
  <div class="hello">
    <div class="row">
      <div class="col-md-3">
        <label for="">ISBN</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="isbn" placeholder="ISBN">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Edition</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="book_edition" placeholder="Edition">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Book Format</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="book_format" placeholder="Book Format">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Number of Page</label>
      </div>
      <div class="col-md-4">
        <input type="number" class="form-control" name="number_of_page" placeholder="Number of Page">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">About</label>
      </div>
      <div class="col-md-9">
        <textarea name="about" class="form-control" rows="4" placeholder="About"></textarea>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Abstract</label>
      </div>
      <div class="col-md-9">
        <textarea name="abstract" class="form-control" rows="4" placeholder="Abstract"></textarea>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Is Abriged?</label>
      </div>
      <div class="col-md-3">
        <select class="form-control" name="abridged">
          <option value="yes">Yes</option>
          <option value="no">No</option>
        </select>
      </div>
    </div>
    <hr>
    <AuthorForm/>
    <PublisherForm/>
  </div>
</template>

<script>
import AuthorForm from './AuthorForm.vue'
import PublisherForm from './PublisherForm'

export default {
  name: 'BookForm',
  components: {
    AuthorForm,
    PublisherForm
  }
}
</script>
