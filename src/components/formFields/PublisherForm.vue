<template>
  <div class="hello">
    <div class="row">
      <div class="col-md-12">
        <h4>Publisher</h4>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Publisher Name</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="publisher_name" placeholder="Publisher Name">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Publisher URL</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="publisher_url" placeholder="Publisher URL">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Publisher Email</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="publisher_email" placeholder="Publisher Email">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Publisher Phone</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="publisher_phone" placeholder="Publisher Phone">
      </div>
    </div>
    <hr>
  </div>
</template>

<script>
export default {
  name: 'PublisherForm'
}
</script>
