<template>
  <div class="firstcomponent">{{first}}</div>
</template>


<script>
export default {
  name: "FirstComponent",
  props: {
    first: String
  }
};
</script>

<style>
.firstcomponent {
  color: red;
  font-size: 56px;
}
</style>
