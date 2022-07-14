<template>
  <div id="global-outer-container" class="">
    <UpperFrame></UpperFrame>
    <ToolBar></ToolBar>
    <ContactMap></ContactMap>
    <SideBar></SideBar>
  </div>
</template>

<script>
import UpperFrame from "@/app/ui/components/upper_ribbon/UpperFrame";
import ToolBar from "@/app/ui/components/toolbar/ToolBar";
import ContactMap from "@/app/ui/components/ContactMap";
import SideBar from "@/app/ui/components/sidebar/SideBar";

export default {
  name: "MainUIComponent",
  components: {SideBar, ContactMap, ToolBar, UpperFrame}
}
</script>

<style scoped>

</style>