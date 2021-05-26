<template>
  <div class="hello">
    <div class="row">
      <div class="col-md-12">
        <h4>Author</h4>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Author Name</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="author_name" placeholder="Author Name">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Author URL</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="author_url" placeholder="Author URL">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Author Email</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="author_email" placeholder="Author Email">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Author Phone</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="author_phone" placeholder="Author Phone">
      </div>
    </div>
    <hr>
  </div>
</template>

<script>
export default {
  name: 'AuthorForm'
}
</script>
