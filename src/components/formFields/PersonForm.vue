<template>
  <div class="hello">
    <div class="row">
      <div class="col-md-3">
        <label for="">ID</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="id" placeholder="Example: www.example.com/users/1">
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
        <label for="">Job Title</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="job_title" placeholder="Job Title">
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
        <label for="">Email</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="email" placeholder="Email">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Phone</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="phone" placeholder="Phone">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Birth Date</label>
      </div>
      <div class="col-md-9">
        <input type="date" class="form-control" name="birth_date" placeholder="Birth Date">
      </div>
    </div>
    <AddressForm/>
  </div>
</template>

<script>
import AddressForm from './AddressForm.vue'
export default {
  name: 'PersonForm',
  components: {
    AddressForm
  }
}
</script>
