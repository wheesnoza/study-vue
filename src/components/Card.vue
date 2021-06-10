<template>
  <div class="card" style="width: 18rem;">
    <img :src="image_path" class="card-img-top">
    <div class="card-body">
      <h5 class="card-title">{{ title }}</h5>
      <p class="card-text">{{ text }}</p>
      <a :href="url" class="btn btn-primary">{{ btn }}</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: [
      "title",
      "text",
      "url",
      "image_path",
      "btn"
  ]
}
</script>