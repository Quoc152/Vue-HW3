<script setup>
  import { ref } from 'vue';

  const string = ref('Hello World!');
  const myClass = ref('example');
  const user = ref({
    name: 'Ho Van Teo',
    age: 21,
  });
</script>

<template>
  <div class="greetings">
    <h3 :class="myClass">String: {{ string }}</h3>
    <p>Tên: {{ user.name }}</p>
    <p>Tuổi: {{ user.age }}</p>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 30px;
}

p {
  font-size: 20px;
}

.example {
  font-size: 20px;
  color: #f70d0d;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
