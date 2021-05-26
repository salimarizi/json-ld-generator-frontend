<template>
  <div class="hello">
    <div class="row">
      <div class="col-md-12">
        <h4>Director</h4>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Director Name</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="director_name" placeholder="Director Name">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Director URL</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="director_url" placeholder="Director URL">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Director Email</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="director_email" placeholder="Director Email">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Director Phone</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="director_phone" placeholder="Director Phone">
      </div>
    </div>
    <hr>
  </div>
</template>

<script>
export default {
  name: 'DirectorForm'
}
</script>
