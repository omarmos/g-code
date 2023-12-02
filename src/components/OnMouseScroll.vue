<template>
    <section class="container">
        <h1 class="title">Excel Code 🦊 Excel Code 🐶 Excel Code 🦊 Excel Code 🐶 .</h1>
    </section>
</template>


<script>
import { renderScene } from "../js/mouse.js"

export default {
  mounted() {
    renderScene()
  }
}
</script>

<style lang="scss">
.container {
    overflow: hidden;
    background: #FFF;
    cursor: ew-resize;
    white-space: nowrap;
    padding: 0vh 0;
}

.title {
    font: bold normal 12vw/1.2 "Montserrat", sans-serif;
    position: relative;
    color: #000;
    display: inline-block;
    margin: 0;
    padding: 0 15%;
    will-change: transform;
}

</style>