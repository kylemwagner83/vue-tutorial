<script>
  export default {
    data() {
      return {
        text: ''
      }
    },
    // methods: {
    //   onInput(e) {
    //     this.text = e.target.value
    //   }
    // }
  }
  </script>
  
  <template>
    <!-- <input :value="text" @input="onInput" placeholder="Type here"> -->

    <input v-model="text" placeholder="Type here">
    <!-- v-model automatically syncs the input value with the bound state,
      so the event handler isn't required -->
      
    <p>{{ text }}</p>
  </template>