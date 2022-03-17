<template>
  <div>
   <span className="user">
          <span className="name">{{name}}</span>
          <span className="handle">{{handle}}</span>
        </span>
  </div>
</template>

<script>import { useSSRContext } from "vue";

export default {
  name: "User",
  props:{
    name: String,
    handle: String,
  }
  

}
</script>

<style>

</style>