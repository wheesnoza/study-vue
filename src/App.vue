<template>
  <div class="container">
    <div class="row">
      <div class="col">
        <Title title="Vue"></Title>
        <Title title="Friend"></Title>
        <Card title="Vue" text="Vue." ref="Go to" url="/some_url" image_path="https://cdn.pixabay.com/photo/2021/02/17/19/48/flower-6025206_1280.jpg"></Card>
      </div>
      <div class="col">
        <Title title="Vue"></Title>
        <Title title="Friend"></Title>
        <Card title="Vue" text="Vue is." ref="Go to" url="/some_url" image_path="https://cdn.pixabay.com/photo/2021/02/17/19/48/flower-6025206_1280.jpg"></Card>
      </div>
      <div class="col">
        <Title title="Vue"></Title>
        <Title title="Friend"></Title>
        <Card title="Vue" text="Vue is awesome." ref="Go to" url="/some_url" image_path="https://cdn.pixabay.com/photo/2021/02/17/19/48/flower-6025206_1280.jpg"></Card>
      </div>
      <div class="col">
        <Title title="Vue"></Title>
        <Title title="Friend"></Title>
        <Card title="Vue" text="Vue is awesome." ref="Go to" url="/some_url" image_path="https://cdn.pixabay.com/photo/2021/02/17/19/48/flower-6025206_1280.jpg"></Card>
      </div>
    </div>
  </div>
</template>

<script>
import Title from './components/Title.vue'
import Card from './components/Card.vue'

export default {
  name: 'App',
  components: {
    Title,
    Card
  }
}
</script>