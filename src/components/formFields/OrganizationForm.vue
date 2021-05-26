<template>
  <div class="hello">
    <div class="row">
      <div class="col-md-3">
        <label for="">Type</label>
      </div>
      <div class="col-md-9">
        <select class="form-control" name="organization_type">
          <option v-for="option in options" :value="option.value" :key="option.value">{{ option.title }}</option>
        </select>
      </div>
    </div>
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
    <div class="row">
      <div class="col-md-3">
        <label for="">Email</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="email" placeholder="Email">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Telephone</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="telephone" placeholder="Telephone">
      </div>
    </div>
    <AddressForm/>
  </div>
</template>

<script>
import AddressForm from './AddressForm.vue'
export default {
  name: 'OrganizationForm',
  components: {
    AddressForm
  },
  data() {
    return {
      options: [
          {value: 'Organization', title: 'Organization'},
          {value: 'Corporation', title: 'Corporation'},
          {value: 'EducationalOrganization', title: 'Educational Organization'},
          {value: 'GovernmentOrganization', title: 'Government Organization'},
          {value: 'LocalBusiness', title: 'Local Business'},
          {value: 'NGO', title: 'NGO'},
          {value: 'PerformingGroup', title: 'Performing Group'},
          {value: 'SportsTeam', title: 'Sports Team'}
      ]
    }
  }
}
</script>
