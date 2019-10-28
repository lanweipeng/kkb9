<template lang="">
    <div>{{someval}}
    <input :type='type' :value='value' @input="onInput"/>
    </div>
</template>
<script>
export default {
  inject: ["someval"],
  props: {
    value: {
      type: String,
      default: ""
    },
    type: {
      type: String,
      default: "text"
    }
  },
  data() {
    return {
      //   value: ""
    };
  },
  methods: {
    onInput(e) {
      let value = e.target.value;
      this.$emit("input", value);
    }
  }
};
</script>