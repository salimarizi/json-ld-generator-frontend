<template>
  <div class="hello">
    <div class="row">
      <div class="col-md-3">
        <label for="">Recipe Name</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="recipe_name" placeholder="Recipe Name">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Recipe Category</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="recipe_category" placeholder="Recipe Category">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Cook Time</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="duration_name" placeholder="Cook Time">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Cooking Method</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="cooking_method" placeholder="Cooking Method">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Cuisine</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="cuisine" placeholder="Cuisine">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Ingridients</label>
      </div>
      <div class="col-md-9">
        <textarea name="ingredients" class="form-control" rows="4" placeholder="Ingridients"></textarea>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Instructions</label>
      </div>
      <div class="col-md-9">
        <textarea name="instructions" class="form-control" rows="4" placeholder="Instructions"></textarea>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Suitable for Diet</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="suitable_for_diet" placeholder="Suitable for Diet">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Recipe Description</label>
      </div>
      <div class="col-md-9">
        <textarea name="recipe_description" class="form-control" rows="4" placeholder="Recipe Description"></textarea>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Recipe Keywords</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="recipe_keywords" placeholder="Recipe Keywords">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Step</label>
      </div>
      <div class="col-md-9">
        <textarea name="step" class="form-control" rows="4" placeholder="Step"></textarea>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Nutrition</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="nutrition_name" placeholder="Nutrition">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Calories</label>
      </div>
      <div class="col-md-4">
        <input type="number" class="form-control" name="nutrition_calories" placeholder="Calories">
      </div>
    </div>
    <RatingForm isAggregate="true"/>
    <AuthorForm/>
    <ThumbnailForm/>
    <div class="row">
      <div class="col-md-12">
        <h4>Video</h4>
      </div>
    </div>
    <VideoComponent/>
  </div>
</template>

<script>
import ThumbnailForm from './ThumbnailForm.vue'
import AuthorForm from './AuthorForm.vue'
import RatingForm from './RatingForm.vue'
import VideoComponent from './VideoComponent.vue'

export default {
  name: 'RecipeForm',
  components: {
    ThumbnailForm,
    AuthorForm,
    VideoComponent,
    RatingForm
  }
}
</script>
