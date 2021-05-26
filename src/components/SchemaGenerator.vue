<template>
  <div class="container">
    <div class="row">
      <div class="col-md-12 text-center">
        <h2>JSON LD Generator {{ json_type }}</h2>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <form id="form-schema" method="post">
          <div class="row">
            <div class="col-md-3">
              <label>Type</label>
            </div>
            <div class="col-md-9">
              <select name="json_type" id="json_type" v-model="json_type" class="form-control">
                <option value="Organization">Organization</option>
                <option value="Product">Product</option>
                <option value="Events">Event</option>
                <option value="LocalBusiness">Local Business</option>
                <option value="Restaurant">Restaurant</option>
                <option value="Recipe">Recipe</option>
                <option value="Article">Article</option>
                <option value="Review">Review</option>
                <option value="Movie">Movie</option>
                <option value="VideoObject">Video Object</option>
                <option value="Person">Person</option>
                <option value="Brand">Brand</option>
                <option value="Book">Book</option>
              </select>
            </div>
          </div>
          <PersonForm v-if="json_type == 'Person'"/>
          <EventForm v-if="json_type == 'Events'"/>
          <ReviewForm v-if="json_type == 'Review'"/>
          <ProductForm v-if="json_type == 'Product'"/>
          <BrandForm v-if="json_type == 'Brand'"/>
          <BookForm v-if="json_type == 'Book'"/>
          <ArticleForm v-if="json_type == 'Article'"/>
          <OrganizationForm v-if="json_type == 'Organization'"/>
          <VideoObjectForm v-if="json_type == 'VideoObject'"/>
          <MovieForm v-if="json_type == 'Movie'"/>
          <RecipeForm v-if="json_type == 'Recipe'"/>
          <LocalBusinessForm v-if="json_type == 'LocalBusiness'"/>
          <LocalBusinessForm v-if="json_type == 'Restaurant'" isRestaurant="true"/>

          <div class="row">
            <div class="col-md-12">
              <br>
              <button type="button" id="btnSubmit" @click="submitForm" class="btn btn-primary pull-right">Submit</button>
            </div>
          </div>
        </form>
      </div>
      <div class="col-md-6">
        <textarea name="result" id="result" v-model="result" readonly class="form-control" rows="42"></textarea>
      </div>
    </div>
  </div>
</template>

<script>
import axios from 'axios'
import PersonForm from './formFields/PersonForm.vue'
import EventForm from './formFields/EventForm.vue'
import ReviewForm from './formFields/ReviewForm.vue'
import ProductForm from './formFields/ProductForm.vue'
import BrandForm from './formFields/BrandForm.vue'
import BookForm from './formFields/BookForm.vue'
import ArticleForm from './formFields/ArticleForm.vue'
import OrganizationForm from './formFields/OrganizationForm.vue'
import VideoObjectForm from './formFields/VideoObjectForm.vue'
import MovieForm from './formFields/MovieForm.vue'
import RecipeForm from './formFields/RecipeForm.vue'
import LocalBusinessForm from './formFields/LocalBusinessForm.vue'

export default {
  name: 'SchemaGenerator',
  props: {
    msg: String
  },
  components: {
    PersonForm,
    EventForm,
    ReviewForm,
    ProductForm,
    BrandForm,
    BookForm,
    ArticleForm,
    OrganizationForm,
    VideoObjectForm,
    MovieForm,
    RecipeForm,
    LocalBusinessForm
  },
  data() {
    return {
      json_type: '',
      result: ''
    }
  },
  methods: {
    submitForm() {
      let form = document.getElementById('form-schema')
      let data = new FormData(form)

      axios.defaults.headers.common['Access-Control-Allow-Origin'] = '*'

      axios.post('http://localhost:5000/schema', data)
       .then(response => {
         this.result = JSON.stringify(response.data, null, "\t")
       })
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h3 {
    margin: 40px 0 0;
  }
  ul {
    list-style-type: none;
    padding: 0;
  }
  li {
    display: inline-block;
    margin: 0 10px;
  }
  a {
    color: #42b983;
  }
</style>
