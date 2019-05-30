<template>
  <div class="grid">
    <div class="block" v-for="cell in cells">
      <HexagonBlock v-bind:text="cell"/>
    </div>
  </div>
</template>

<script>
import HexagonBlock from "./components/HexagonBlock";

export default {
  
  data() {
    return { count: 0, 
    cells: [0, 1, 2, 3, 4,5,6,7,8,9,0,1,2,3,4,2,32,32,21,23,32,2,23,32,3,32,23,32,2,2,2] };
  },
  methods: {
    increment: function() {
      this.count++;
    },
    decrement: function() {
      this.count--;
    }
  },
  components: {
    HexagonBlock
  }
};
</script>
