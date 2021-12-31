<template>
  <div class="body-sec">
    <div class="body-bg-image">
      <img
        class="star-bg-image"
        :src="require(`../../assets/star_background.png`)"
        alt="Fragcolor Star Background"
      />
    </div>

    <div id="filter-sec">
      <p>filter</p>

      <!-- <Dropdown
      :options="[{ id: 1, name: 'Option 1'}, { id: 2, name: 'Option 2'}]"
      v-on:selected="validateSelection"
      v-on:filter="getDropdownValues"
      :disabled="false"
      name="zipcode"
      :maxItem="10"
      placeholder="Please select an option">
    </Dropdown> -->
    </div>

    <div id="product-sec">
      <div class="asset-holder">
        <div class="asset-img-holder">
          <img
            class="asset-display-image"
            :src="require(`../../assets/dreams_img_test.jpeg`)"
            alt="asset display image"
          />
        </div>

        <div class="asset-desc-holder">
          <p>Southpaw Cooking</p>
        </div>
      </div>

      <div class="asset-holder">
        <div class="asset-img-holder">
          <img
            class="asset-display-image"
            :src="require(`../../assets/dreams_img_test.jpeg`)"
            alt="asset display image"
          />
        </div>

        <div class="asset-desc-holder">
          <p>Southpaw Cooking</p>
        </div>
      </div>

      <div class="asset-holder">
        <div class="asset-img-holder">
          <img
            class="asset-display-image"
            :src="require(`../../assets/dreams_img_test.jpeg`)"
            alt="asset display image"
          />
        </div>

        <div class="asset-desc-holder">
          <p>Southpaw Cooking</p>
        </div>
      </div>

      <div class="asset-holder">
        <div class="asset-img-holder">
          <img
            class="asset-display-image"
            :src="require(`../../assets/dreams_img_test.jpeg`)"
            alt="asset display image"
          />
        </div>

        <div class="asset-desc-holder">
          <p>Southpaw Cooking</p>
        </div>
      </div>

      <div class="asset-holder">
        <div class="asset-img-holder">
          <img
            class="asset-display-image"
            :src="require(`../../assets/dreams_img_test.jpeg`)"
            alt="asset display image"
          />
        </div>

        <div class="asset-desc-holder">
          <p>Southpaw Cooking</p>
        </div>
      </div>
    </div>

    <!-- component :is="currentView" class="body-template" /-->
  </div>
</template>

<!--script type="text/javascript">
  Vue.use(Dropdown);
</script-->
<script>
// import { Component, Prop, Vue, Watch } from 'vue-property-decorator';
import Vue from "vue";
// import assetSec from "../sections/AssetDisplaySec.vue";
import Dropdown from "vue-simple-search-dropdown";

// Vue.component('Dropdown', Dropdown);

// Vue.use(Dropdown);

export default {
  name: "BodyTemplate",
  props: {
    currentView: {
      type: Object,
      default: null,
    },
  },
  components: {
    // "asset-sec": assetSec,
    Dropdown: Dropdown,
  },
};
</script>

<style scoped>
.body-template {
  width: 100%;
}

#filter-sec {
  display: block;
  /* margin-top: 70px; */
  /* background-color: darkslateblue; */
}

#filter-sec p {
  color: white !important;
  padding-top: 92px;
  z-index: 1;
  /* background: antiquewhite; */
  position: relative;
}

#product-sec {
  display: block;
  width: 80vw;
  margin-left: auto;
  margin-right: auto;
}

.body-bg-image {
  //display: inline;
  position: fixed;
  z-index: -1;
  width: 100%;
}

.star-bg-image {
  width: 100%;
  height: 150vh;
  object-fit: cover;
}

.asset-holder {
  margin-right: 2vw;
  margin-bottom: 2vw;
  display: inline-block;
}

.asset-display-image {
  width: 18vw;
  border-radius: 8px;
  border: 1px solid #333;
}

.asset-desc-holder p {
  color: white;
}
</style>
