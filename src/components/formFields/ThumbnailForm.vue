<template>
  <div class="hello">
    <div class="row">
      <div class="col-md-12">
        <h4>Thumbnail</h4>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Thumbnail Name</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="image_object_name" placeholder="Thumbnail Name">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Thumbnail URL</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="image_object_url" placeholder="Thumbnail URL">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Thumbnail Caption</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="image_object_caption" placeholder="Thumbnail Caption">
      </div>
    </div>
    <hr>
  </div>
</template>

<script>
export default {
  name: 'ThumbnailForm'
}
</script>
