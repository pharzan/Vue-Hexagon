
<template>
		<div class="block">{{text}}</div>
</span>
</template>


<script>
export default {
  props:['text'],
  data() {
    return {
      msg: "No messages",
    };
  },
  methods: {
    message: function() {
      this.msg = "New message!!!";
    },
    inputUpdate: function(e) {
      console.log(e);
      this.msg += e.data;
    }
  },
 
};
</script>
