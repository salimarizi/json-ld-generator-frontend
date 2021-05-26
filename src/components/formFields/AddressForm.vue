<template>
  <div class="hello">
    <div class="row">
      <div class="col-md-3">
        <label for="">Address</label>
      </div>
      <div class="col-md-9">
        <textarea name="address" class="form-control" rows="4" placeholder="Address"></textarea>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">City</label>
      </div>
      <div class="col-md-4">
        <input type="text" class="form-control" name="city" placeholder="City">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">PO. Box</label>
      </div>
      <div class="col-md-3">
        <input type="text" class="form-control" name="po_box" placeholder="PO. Box">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Region</label>
      </div>
      <div class="col-md-4">
        <input type="text" class="form-control" name="region" placeholder="Region">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Postal Code</label>
      </div>
      <div class="col-md-3">
        <input type="text" class="form-control" name="postal_code" placeholder="Postal Code">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Country</label>
      </div>
      <div class="col-md-4">
        <input type="text" class="form-control" name="country" placeholder="Country">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AddressForm'
}
</script>
