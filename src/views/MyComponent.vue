<template>
  <div>
    <!-- <h2>{{ title }}</h2>
    <p>{{ message }}</p>
    <button @click="onClick">{{ buttonText }}</button> -->
    <input :type="type" />
    <h3>{{ name }}</h3>
    
  </div>
</template>

<script>
export default {
  name: 'MyComponent',
  props: {
    type: {
      type: String
    },
    name: {
      type: String
    }
  },
  data() {
    return {
      msg: 'Hello'
    }
  },
  methods: {
    onClick() {
      // Handle click event here
    }
  }
}
</script>