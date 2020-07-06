<template>
<b-container>
<b-form inline class="d-flex justify-content-center">
    <label class="sr-only" for="inline-form-input-name" >Name</label>
    <b-input
      v-model="itemSearch"
      id="inline-form-input-name"
      class="mb-2 mr-sm-2 mb-sm-0 "
      placeholder="Search Books"
    ></b-input>
    <router-link to="/searchResult"><b-button variant="primary">Search</b-button></router-link>
  </b-form>
  </b-container>

</template>

<script>
export default {
  props: {
    itemSearch: {
      type: String,
      default: ''
    }
  },
  data () {
    return {
    }
  }
}
</script>
