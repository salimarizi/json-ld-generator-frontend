<template>
  <div class="hello">
    <div class="row" v-if="!isRestaurant">
      <div class="col-md-3">
        <label for="">Business Type</label>
      </div>
      <div class="col-md-9">
        <select class="form-control" name="business_type">
          <option v-for="option in options" :value="option.value" :key="option.value">{{ option.title }}</option>
        </select>
      </div>
    </div>
    <input type="hidden" name="business_type" value="Restaurant" v-else>
    <div class="row">
      <div class="col-md-3">
        <label for="">Name</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="name" placeholder="Name">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">URL</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="url" placeholder="URL">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Logo</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="logo" placeholder="Logo">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Image</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="image" placeholder="Image">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Description</label>
      </div>
      <div class="col-md-9">
        <textarea name="description" class="form-control" rows="4" placeholder="Description"></textarea>
      </div>
    </div>
    <AddressForm/>
    <div class="row">
      <div class="col-md-3">
        <label for="">Phone</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="telephone" placeholder="Phone">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Opening Hours</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="opening_hours" placeholder="Opening Hours">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Contact Type</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="contact_type" placeholder="Contact Type">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Price Range</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="price_range" placeholder="Price Range">
      </div>
    </div>
    <div class="row" v-if="isRestaurant">
      <div class="col-md-3">
        <label for="">Serves Cuisine</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="serves_cuisine" placeholder="Serves Cuisine">
      </div>
    </div>
  </div>
</template>

<script>
import AddressForm from './AddressForm.vue'
export default {
  name: 'LocalBusinessForm',
  props: {
    isRestaurant: Boolean
  },
  components: {
    AddressForm
  },
  data() {
    return {
      options: [
          {value: 'LocalBusiness', title: 'Local Business'},
      		{value: 'AutomotiveBusiness', title: 'Automotive Business'},
      		{value: 'EntertainmentBusiness', title: 'Entertainment Business'},
      		{value: 'HealthAndBeautyBusiness', title: 'Health And Beauty Business'},
      		{value: 'HomeAndConstruction', title: 'Home And Construction'},
      		{value: 'HVACBusiness', title: 'HVAC Business'},
      		{value: 'LodgingBusiness', title: 'Lodging Business'}
      ]
    }
  }
}
</script>
