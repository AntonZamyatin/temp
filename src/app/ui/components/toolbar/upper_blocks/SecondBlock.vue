<template>
  <div class="block-of-buttons">
    <button class="btn btn-outline-primary" type="button"><i class="bi bi-arrow-repeat"></i></button>
    <button class="btn btn-outline-primary" type="button"><i class="bi bi-arrows-move"></i></button>
  </div>
</template>

<script>
export default {
  name: "SecondBlock"
}
</script>

<style scoped>
.block-of-buttons {
  /* block of buttons2 */

  /* Auto layout */
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding: 0px;
  gap: 4px;

  width: 44px;
  height: 76px;


  /* Inside auto layout */
  flex: none;
  order: 1;
  flex-grow: 0;
}
</style>