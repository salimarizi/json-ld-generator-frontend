<template>
  <div class="hello">
    <div class="row">
      <div class="col-md-12">
        <h4>Actor</h4>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Actor Name</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="actor_name" placeholder="Actor Name">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Actor URL</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="actor_url" placeholder="Actor URL">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Actor Email</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="actor_email" placeholder="Actor Email">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Actor Phone</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="actor_phone" placeholder="Actor Phone">
      </div>
    </div>
    <hr>
  </div>
</template>

<script>
export default {
  name: 'ActorForm'
}
</script>
