<template>
  <div class="hello">
    <ActorForm/>
    <DirectorForm/>
    <MusicForm/>
    <ThumbnailForm/>
    <VideoComponent/>
  </div>
</template>

<script>
import ActorForm from './ActorForm.vue'
import DirectorForm from './DirectorForm.vue'
import MusicForm from './MusicForm.vue'
import ThumbnailForm from './ThumbnailForm.vue'
import VideoComponent from './VideoComponent.vue'
export default {
  name: 'VideoObjectForm',
  components: {
    ActorForm,
    DirectorForm,
    MusicForm,
    ThumbnailForm,
    VideoComponent
  }
}
</script>
