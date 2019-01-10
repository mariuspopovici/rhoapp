<template>
  <button class="btn btn-info" type="button" :disabled="loading">
    <div id="loadingButton" v-if="loading">
      <font-awesome-icon icon="spinner" spin/>&nbsp;Please wait...
    </div>
    <div id="loadingButton" v-else>
      <font-awesome-icon icon="location-arrow"/>&nbsp;My Location
    </div>
  </button>
</template>

<script>
export default {
  props: {
    loading: { type: Boolean }
  }
};
</script>