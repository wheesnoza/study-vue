<template>
  <div>
    <h1>Welcome {{ title }}</h1>
    <Subtitle></Subtitle>
  </div>
</template>

<script>
import Subtitle from './Subtitle.vue'

export default {
  props:[
      "title"
  ],
  name: "Title",
  components: {
    Subtitle
  }
}
</script>