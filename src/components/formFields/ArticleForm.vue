<template>
  <div class="hello">
    <div class="row">
      <div class="col-md-3">
        <label for="">Name</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="article_name" placeholder="Name">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Body</label>
      </div>
      <div class="col-md-9">
        <textarea name="article_body" class="form-control" rows="4" placeholder="Body"></textarea>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Section</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="article_section" placeholder="Section">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Headline</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="headline" placeholder="Headline">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Published</label>
      </div>
      <div class="col-md-9">
        <input type="date" class="form-control" name="date_published" placeholder="Published">
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
        <label for="">Backstory</label>
      </div>
      <div class="col-md-9">
        <textarea name="backstory" class="form-control" rows="4" placeholder="Backstory"></textarea>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Page</label>
      </div>
      <div class="col-md-4">
        <input type="text" class="form-control" name="page_start" placeholder="Page Start">
      </div>
      <div class="col-md-4">
        <input type="text" class="form-control" name="page_end" placeholder="Page End">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Pagination</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="pagination" placeholder="Pagination">
      </div>
    </div>
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
        <label for="">Word Count</label>
      </div>
      <div class="col-md-4">
        <input type="number" class="form-control" name="word_count" placeholder="Word Count">
      </div>
    </div>
    <hr>
    <div class="row">
      <div class="col-md-12">
        <h4>Author</h4>
      </div>
    </div>
    <AuthorForm/>
    <hr>
    <div class="row">
      <div class="col-md-12">
        <h4>Publisher</h4>
      </div>
    </div>
    <OrganizationForm/>
  </div>
</template>

<script>
import AuthorForm from './AuthorForm.vue'
import OrganizationForm from './OrganizationForm.vue'

export default {
  name: 'ArticleForm',
  components: {
    AuthorForm,
    OrganizationForm
  }
}
</script>
