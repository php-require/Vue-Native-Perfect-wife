<template>
  <view class="container">
    <text class="text-color-primary">My Vue Native App</text>
     <touchable-opacity :on-press="onPressButton">
      <image
        :style="{alignItems: 'center', backgroundColor: '#DDDDDD'}"
        :source="require('./assets/favicon.png' )"
      />
    </touchable-opacity>
  </view>
</template>

<style>
.container {
  background-color: white;
  align-items: center;
  justify-content: center;
  flex: 1;
}
.text-color-primary {
  color: blue;
}
</style>
<script>
    export default {
        methods: {
            onPressButton: function() {
                alert('Clicked Image')
            }
        }
    }
</script>