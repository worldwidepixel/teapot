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
        statusCode: 500,
        fatal: false,
        message: "Internal Server Error (Chai not supported)",
      })
    }
  }  }
</script>