<template>
  <div class="hello">
    <div class="row">
      <div class="col-md-3">
        <label for="">Type</label>
      </div>
      <div class="col-md-9">
        <select class="form-control" name="event_type">
          <option v-for="option in options" :value="option.value" :key="option.value">{{ option.title }}</option>
        </select>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">ID</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="id" placeholder="Example: www.example.com/events/1">
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
        <label for="">Start Date</label>
      </div>
      <div class="col-md-9">
        <input type="datetime-local" class="form-control" name="start_date" placeholder="Start Date">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">End Date</label>
      </div>
      <div class="col-md-9">
        <input type="datetime-local" class="form-control" name="end_date" placeholder="End Date">
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
        <label for="">Attendance Mode</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="attendance_mode" placeholder="Attendance Mode">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Event Status</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="event_status" placeholder="Event Status">
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
    <hr>
    <OfferForm/>
    <div class="row">
      <div class="col-md-3">
        <label for="">Venue Name</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="venue_name" placeholder="Venue Name">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Venue URL</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="venue_url" placeholder="Venue URL">
      </div>
    </div>
    <AddressForm/>
  </div>
</template>

<script>
import OfferForm from './OfferForm'
import AddressForm from './AddressForm'

export default {
  name: 'EventForm',
  components: {
    OfferForm,
    AddressForm
  },
  data() {
    return {
      options: [
          {value: 'Event', title: 'Event'},
      		{value: 'BusinessEvent', title: 'Business Event'},
      		{value: 'ChildrenEvent', title: 'Children Event'},
      		{value: 'ComedyEvent', title: 'Comedy Event'},
      		{value: 'DanceEvent', title: 'Dance Event'},
      		{value: 'EducationalEvent', title: 'Educational Event'},
      		{value: 'Festival', title: 'Festival'},
      		{value: 'FoodEvent', title: 'Food Event'},
      		{value: 'LiteraryEvent', title: 'Literary Event'},
      		{value: 'MusicEvent', title: 'Music Event'},
      		{value: 'SalesEvent', title: 'Sales Event'},
      		{value: 'SocialEvent', title: 'Social Event'},
      		{value: 'SportsEvent', title: 'Sports Event'},
      		{value: 'TheaterEvent', title: 'Theater Event'},
      		{value: 'UserInteraction', title: 'User Interaction'},
      		{value: 'VisualArtsEvent', title: 'Visual Arts Event'}
      ]
    }
  }
}
</script>
