<template>
  <div class="header-ribbon">
    <div id="left-header-block" class="input-group">
      <div id="search-container">
        <div id="search-input-group" class="input-group input-group-sm mb-3">
          <input id="global-search-input" class="form-control form-control-sm" placeholder="I'm looking for..."
                 type="text">
          <button id="global-search-button" class="btn btn-sm btn-outline-light" type="button">Go to</button>
        </div>
      </div>
      <div class="mb-3">
        <select class="form-select form-select-sm">
          <option selected>Contigs All</option>
          <option value="1">ctgA</option>
          <option value="2">ctgB</option>
          <option value="3">ctgC</option>
        </select>
      </div>
      <div class="mb-3">
        <select class="form-select form-select-sm">
          <option selected value="0">Contigs All</option>
          <option value="1">ctgA</option>
          <option value="2">ctgB</option>
          <option value="3">ctgC</option>
        </select>
      </div>
      <div class="mb-3">
        <select class="form-select form-select-sm">
          <option selected value="0">Show Observed</option>
          <option value="1">Show Expected</option>
        </select>
      </div>
      <div class="mb-3">
        <select class="form-select form-select-sm">
          <option selected value="0">Normalization None</option>
          <option value="1">Normalization Cooler</option>
        </select>
      </div>
    </div>
    <div id="right-header-block" class="input-group">
      <button id="reload-tiles-button" class="btn-sm btn-outline-primary" type="button">Reload tiles</button>
      <button id="export-png-button" class="btn-sm btn-outline-primary" type="button"><i class="bi bi-box-arrow-up"></i>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderRibbon"
}
</script>

<style scoped>
.header-ribbon {
  /* header */

  /* Auto layout */
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  padding: 12px 16px;
  gap: 16px;

  width: 1440px;
  height: 53px;

  /* Global/02. Secondary */
  background: #6C757D;

  /* Inside auto layout */
  flex: none;
  order: 1;
  flex-grow: 0;
}

#left-header-block {
  /* left block */

  /* Auto layout */
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  padding: 0px;
  gap: 16px;

  width: 920px;
  height: 29px;


  /* Inside auto layout */
  flex: none;
  order: 0;
  flex-grow: 0;
}

#search-container {
  /* search */

  /* Auto layout */
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding: 0px 16px 0px 0px;
  gap: 10px;

  width: 216px;
  height: 29px;


  /* Inside auto layout */
  flex: none;
  order: 0;
  flex-grow: 0;
}

#search-input-group {
  /* Input group */

  box-sizing: border-box;

  /* Auto layout */
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  padding: 0px;

  width: 200px;
  height: 29px;

  /* Global/09. White */
  /*background: #FFFFFF;*/

  /* Components/Forms/Input border */
  /*border: 1px solid #CED4DA;*/
  border-radius: 4px;

  /* Inside auto layout */
  flex: none;
  order: 0;
  flex-grow: 0;
}

#right-header-block {
  /* right block */

  /* Auto layout */
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  padding: 0px;
  gap: 16px;

  width: 150px;
  height: 29px;


  /* Inside auto layout */
  flex: none;
  order: 1;
  flex-grow: 0;
}

#reload-tiles-button {
  /* _base */

  box-sizing: border-box;

  /* Auto layout */
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 4px 8px;

  font-family: 'Roboto', ui-sans-serif;
  font-style: normal;
  font-weight: 100;
  font-size: 14px;
  line-height: 21px;

  text-align: center;

  width: 90px;
  height: 29px;

  /* Global/07. Light */
  border: 1px solid #F8F9FA;
  border-radius: 4px;

  /* Inside auto layout */
  flex: none;
  order: 0;
  flex-grow: 0;
}

#export-png-button {
  /* _base */

  box-sizing: border-box;

  /* Auto layout */
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 4px 8px;

  width: 37px;
  height: 29px;

  /* Global/07. Light */
  border: 1px solid #F8F9FA;
  border-radius: 4px;

  /* Inside auto layout */
  flex: none;
  order: 1;
  flex-grow: 0;
}

</style>