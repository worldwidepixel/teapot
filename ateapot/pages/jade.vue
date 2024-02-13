<template>
    <title> I am a teapot. </title>
    <div class="a"></div>
</template>

<style>

.a {
    font-family: sans-serif;
}

</style>
  
<script>
  export default {
    async setup() {
    if (true) {
      throw createError({
        statusCode: 507,
        fatal: false,
        message: "Insufficient Storage",
      })
    }
  }  }
</script>