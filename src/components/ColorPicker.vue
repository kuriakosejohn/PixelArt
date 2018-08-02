<template>
  <div>
    <Pixel interactive color="white" current="true"/>
    <Pixel interactive color="lightblue" current="color == 'lightblue' ? true : false"/>
    <Pixel interactive color="blue" current="color == 'blue' ? true : false"/>
    <Pixel interactive color="darkblue" current="color == 'darkblue' ? true : false"/>
    {{color}}
  </div>
</template>

<script>
import Pixel from "./Pixel";

export default {
  name: "ColorPicker",
  props: {
    color: String
  },
  methods: {
    changeColor: function(color) {
      alert(color);
    }
  },
  components: {
    Pixel
  }
};
</script>
