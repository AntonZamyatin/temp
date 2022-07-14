<template>
  <div class="toolbar-outer">
    <div class="toolbar-upper">
      <FirstBlock></FirstBlock>
      <SecondBlock></SecondBlock>
      <ThirdBlock></ThirdBlock>
    </div>
    <div class="toolbar-bottom">
      <BottomButtons></BottomButtons>
    </div>
  </div>
</template>

<script>
import FirstBlock from "@/app/ui/components/toolbar/upper_blocks/FirstBlock";
import SecondBlock from "@/app/ui/components/toolbar/upper_blocks/SecondBlock";
import ThirdBlock from "@/app/ui/components/toolbar/upper_blocks/ThirdBlock";
import BottomButtons from "@/app/ui/components/toolbar/bottom_blocks/BottomButtons";

export default {
  name: "ToolBar",
  components: {BottomButtons, ThirdBlock, SecondBlock, FirstBlock},
  data: function () {
    return {
      button_blocks: [FirstBlock, SecondBlock, ThirdBlock],
    }
  }
}
</script>

<style scoped>
.toolbar-outer {
  /* Auto layout */
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  padding: 16px 4px;
  gap: 6px;

  /*position: absolute;*/
  position: absolute;
  float: left;
  width: 60px;
  height: 915px;
  left: 0px;
  top: 109px;

  /* Global/07. Light */
  background: #F8F9FA;

  /* Shadows/02. Regular */
  box-shadow: 0px 8px 16px rgba(0, 0, 0, 0.15);
}

.toolbar-upper {
  /* upper block */

  /* Auto layout */
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding: 0px;
  gap: 24px;

  width: 44px;
  height: 356px;


  /* Inside auto layout */
  flex: none;
  order: 0;
  flex-grow: 0;
}

.toolbar-bottom {
  margin-bottom: 16px;
}
</style>