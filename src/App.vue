<!-- Class binding -->
<!-- <template>
  <h1 
  :class="{ active: isActive }" 
  @click="activate">
    Hello?!({{ isActive }})
  </h1>
</template>

<script>
export default {
  data() {
    return {
      isActive: false
    }
  },
  methods: {
    activate() {
      this.isActive = true
    }
  }
}
</script>

<style scoped>
  .active {
    color: red;
    font-weight: bold;
  } 
</style> -->

<!-- Style Binding: object -->
<!-- <template>
  <h1 
  :style="{
    color,
    fontSize
  }"
  @click="changeStyle">
  Hello?!
  </h1>
</template>

<script>
export default {
  data() {
    return {
      color: 'orange',
      fontSize: '30px'
    }
  },
  methods: {
    changeStyle() {
      this.color = 'red',
      this.fontSize = '50px'
    }
  }
}
</script> -->

<!-- Style Binding: array -->
<template>
  <h1 
  :style="[fontStyle, backgroundStyle]"
  @click="changeStyle">
  Hello?!
  </h1>
</template>

<script>
export default {
  data() {
    return {
      fontStyle: {
        color: 'orange',
        fontSize: '30px'
      },
      backgroundStyle: {
        backgroundColor: 'black'
      }
    }
  },
  methods: {
    changeStyle() {
      this.fontStyle.color = 'red',
      this.fontStyle.fontSize = '50px'
    }
  }
}
</script>
