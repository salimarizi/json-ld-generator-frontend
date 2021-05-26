<template>
  <div class="hello">
    <div class="row">
      <div class="col-md-12">
        <h4>Music By</h4>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Music Group Name</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="music_group_name" placeholder="Music Group Name">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Music Group URL</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="music_group_url" placeholder="Music Group URL">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Music Group Genre</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="music_group_genre" placeholder="Music Group Genre">
      </div>
    </div>
    <hr>
  </div>
</template>

<script>
export default {
  name: 'MusicForm'
}
</script>
