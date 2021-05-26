<template>
  <div class="hello">
    <div class="row">
      <div class="col-md-12">
        <h4>Offer</h4>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Offer URL</label>
      </div>
      <div class="col-md-9">
        <input type="text" class="form-control" name="offer_url" placeholder="Offer URL">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Offer Description</label>
      </div>
      <div class="col-md-9">
        <textarea name="offer_description" class="form-control" rows="4" placeholder="Offer Description"></textarea>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Price and Currency</label>
      </div>
      <div class="col-md-4">
        <input type="text" class="form-control" name="offer_price_currency" placeholder="Offer Currency">
      </div>
      <div class="col-md-4">
        <input type="number" class="form-control" name="offer_price" placeholder="Offer Price">
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Offer Availability</label>
      </div>
      <div class="col-md-9">
        <select class="form-control" name="offer_availability">
          <option value="Discontinued">Discontinued</option>
          <option value="InStock">In Stock</option>
          <option value="InStoreOnly">In Store Only</option>
          <option value="LimitedAvailability">Limited Availability</option>
          <option value="OnlineOnly">Online Only</option>
          <option value="OutOfStock">Out Of Stock</option>
          <option value="PreOrder">Pre Order</option>
          <option value="SoldOut">Sold Out</option>
        </select>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <label for="">Offer Valid From</label>
      </div>
      <div class="col-md-9">
        <input type="date" class="form-control" name="offer_valid_from" placeholder="Offer Valid From">
      </div>
    </div>
    <hr>
  </div>
</template>

<script>
export default {
  name: 'OfferForm'
}
</script>
