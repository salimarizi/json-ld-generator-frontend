<template>
  <div class="hello">
    <div class="row">
      <div class="col-md-3">
        <label for="">Video Name</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="video_name" placeholder="Video Name">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Description</label>
      </div>
      <div class="col-md-9">
        <textarea name="video_description" class="form-control" rows="4"></textarea>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Upload Date</label>
      </div>
      <div class="col-md-9">
        <input type="date" class="form-control" name="upload_date" placeholder="Upload Date">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Video Caption</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="video_caption" placeholder="Video Caption">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Transcript</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="transcript" placeholder="Transcript">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Frame Size</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="frame_size" placeholder="Frame Size">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Quality</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="quality" placeholder="Quality">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Bitrate</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="bitrate" placeholder="Bitrate">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Content URL</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="content_url" placeholder="Content URL">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Embed URL</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="embed_url" placeholder="Embed URL">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'VideoComponent'
}
</script>
