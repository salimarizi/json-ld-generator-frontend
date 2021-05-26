<template>
  <div class="hello">
    <ActorForm/>
    <DirectorForm/>
    <MusicForm/>
    <div class="row">
      <div class="col-md-12">
        <h4>Trailer</h4>
      </div>
    </div>
    <VideoComponent/>
    <hr>
    <ThumbnailForm/>
    <div class="row">
      <div class="col-md-12">
        <h4>Production Company</h4>
      </div>
    </div>
    <OrganizationForm/>
    <hr>
    <div class="row">
      <div class="col-md-3">
        <label for="">Movie Name</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="movie_name" placeholder="Movie Name">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Title EIDR</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="title_eidr" placeholder="Title EIDR">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Subtitle Language</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="subtitle_language" placeholder="Subtitle Language">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Duration</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="duration" placeholder="Duration">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">About</label>
      </div>
      <div class="col-md-9">
        <textarea name="movie_about" class="form-control" rows="4" placeholder="About"></textarea>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Origin Country</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="country_name" placeholder="Origin Country">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Created Date</label>
      </div>
      <div class="col-md-9">
        <input type="date" class="form-control" name="date_created" placeholder="Created Date">
      </div>
    </div>
  </div>
</template>

<script>
import ActorForm from './ActorForm.vue'
import DirectorForm from './DirectorForm.vue'
import MusicForm from './MusicForm.vue'
import OrganizationForm from './OrganizationForm.vue'
import VideoComponent from './VideoComponent.vue'
import ThumbnailForm from './ThumbnailForm.vue'
export default {
  name: 'MovieForm',
  components: {
    ActorForm,
    DirectorForm,
    MusicForm,
    OrganizationForm,
    VideoComponent,
    ThumbnailForm
  }
}
</script>
