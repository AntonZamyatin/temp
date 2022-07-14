<template>
  <aside class="sidebar">
    <div id="upper-block">
      <div id="minimap">

      </div>

      <div id="color-range">

      </div>

      <div id="saved-locations">

      </div>
    </div>

    <div id="layers-block">
      <!-- Instantiate layer components here using v-for -->
      <LayerComponent v-for="layer in layers" v-bind:key="layer.name" v-bind:layer-name="layer.name"></LayerComponent>
    </div>
  </aside>
</template>

<script>
import LayerComponent from "@/app/ui/components/sidebar/LayerComponent";

export default {
  name: "SideBar",
  components: {LayerComponent},
  data: function () {
    return {
      layers: [
        {name: 'Edit'},
        {name: 'Chr'},
        {name: 'Scaff'}
      ]
    }
  }
}
</script>

<style scoped>
.sidebar {
  /* sidebar */

  /* Auto layout */
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  padding: 30px 0px 0px;
  gap: 1px;

  position: absolute;
  width: 232px;
  height: 915px;
  left: 1208px;
  top: 109px;

  /* Global/07. Light */
  background: #F8F9FA;

  /* Shadows/02. Regular */
  box-shadow: 0px 8px 16px rgba(0, 0, 0, 0.15);
}

#upper-block {
  /* upper block */

  /* Auto layout */
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 0px;
  gap: 4px;

  width: 232px;
  height: 731px;


  /* Inside auto layout */
  flex: none;
  order: 0;
  flex-grow: 0;
}

#layers-block {
  /* layers */

  /* Auto layout */
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding: 16px;
  gap: 8px;

  width: 232px;
  height: 108px;

  /* Global/09. White */
  background: #FFFFFF;

  /* Shadows/01. Small */
  box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.075);

  /* Inside auto layout */
  flex: none;
  order: 1;
  flex-grow: 0;
}

#minimap {
  /* map */

  width: 232px;
  height: 232px;


  /* Inside auto layout */
  flex: none;
  order: 0;
  flex-grow: 0;
}

#color-range {
  /* color range */

  /* Auto layout */
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding: 16px;
  gap: 12px;

  width: 232px;
  height: 121px;

  /* Global/09. White */
  background: #FFFFFF;

  /* Shadows/01. Small */
  box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.075);

  /* Inside auto layout */
  flex: none;
  order: 1;
  flex-grow: 0;
}

#saved-locations {
  /* saved locations */

  /* Auto layout */
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 16px 0px;
  gap: 8px;

  width: 232px;
  height: 370px;

  /* Global/09. White */
  background: #FFFFFF;

  /* Shadows/01. Small */
  box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.075);

  /* Inside auto layout */
  flex: none;
  order: 2;
  flex-grow: 0;
}
</style>