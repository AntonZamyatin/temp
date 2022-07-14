<template>
  <div class="upper-frame">
    <NavigationBar></NavigationBar>
    <HeaderRibbon></HeaderRibbon>
  </div>
</template>

<script>
import NavigationBar from "@/app/ui/components/upper_ribbon/NavigationBar";
import HeaderRibbon from "@/app/ui/components/upper_ribbon/HeaderRibbon";

export default {
  name: "UpperFrame",
  components: {HeaderRibbon, NavigationBar}
}
</script>

<style scoped>
.upper-frame {
  /* navbar&header */

  /* Auto layout */
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding: 0px;

  position: absolute;
  width: 1440px;
  height: 109px;
  left: 0px;
  top: 0px;
}
</style>