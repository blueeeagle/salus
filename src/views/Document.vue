<template>
  <ion-page>
    <!-- User -->
   <ion-content :fullscreen="true">     
      <ExploreContainer name="Document page" />
      
      <ion-refresher  slot="fixed" @ionPull="doRefresh($event)">
      <ion-refresher-content></ion-refresher-content>
    </ion-refresher>
    
      <div class="outerPadding">
      <ion-card>
        <ion-row>
          <ion-col size="12">
            <ion-card-title class="plywood-invoice">Plywood Invoice</ion-card-title>
            <ion-card-subtitle class="doc-subtitle"
              >Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent eget velit nunc. Aliquam tempus elit sit amet erat maximus, eu consequat tortor volutpat.</ion-card-subtitle
            >
          </ion-col>
        </ion-row>
        <ion-row class="custom-border-top">
          <ion-col size="7">
            <div class="text-subdarkblue font-weight">Created on: 14 Oct 2021</div>
          </ion-col>
          <ion-col size="5" class="ion-text-center">
            <div class="text-blue">Download Attachment</div>
          </ion-col>
        </ion-row>
      </ion-card>
      <ion-card>
        <ion-row>
          <ion-col size="12">
            <ion-card-title class="plywood-invoice">Plywood Invoice</ion-card-title>
            <ion-card-subtitle class="doc-subtitle"
              >Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent eget velit nunc. Aliquam tempus elit sit amet erat maximus, eu consequat tortor volutpat.</ion-card-subtitle
            >
          </ion-col>
        </ion-row>
        <ion-row class="custom-border-top">
          <ion-col size="7">
            <div class="text-subdarkblue font-weight">Created on: 14 Oct 2021</div>
          </ion-col>
          <ion-col size="5" class="ion-text-center">
            <div class="text-blue">Download Attachment</div>
          </ion-col>
        </ion-row>
      </ion-card>
      <ion-card>
        <ion-row>
          <ion-col size="12">
            <ion-card-title class="plywood-invoice">Plywood Invoice</ion-card-title>
            <ion-card-subtitle class="doc-subtitle"
              >Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent eget velit nunc. Aliquam tempus elit sit amet erat maximus, eu consequat tortor volutpat.</ion-card-subtitle
            >
          </ion-col>
        </ion-row>
        <ion-row class="custom-border-top">
          <ion-col size="7">
            <div class="text-subdarkblue font-weight">Created on: 14 Oct 2021</div>
          </ion-col>
          <ion-col size="5" class="ion-text-center">
            <div class="text-blue">Download Attachment</div>
          </ion-col>
        </ion-row>
      </ion-card>
      <ion-card>
        <ion-row>
          <ion-col size="12">
            <ion-card-title class="plywood-invoice">Plywood Invoice</ion-card-title>
            <ion-card-subtitle class="doc-subtitle"
              >Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent eget velit nunc. Aliquam tempus elit sit amet erat maximus, eu consequat tortor volutpat.</ion-card-subtitle
            >
          </ion-col>
        </ion-row>
        <ion-row class="custom-border-top">
          <ion-col size="7">
            <div class="text-subdarkblue font-weight">Created on: 14 Oct 2021</div>
          </ion-col>
          <ion-col size="5" class="ion-text-center">
            <div class="text-blue">Download Attachment</div>
          </ion-col>
        </ion-row>
      </ion-card>
      </div>
     
    </ion-content>
  </ion-page>
</template>

<script lang="ts">

import { IonPage, IonContent ,IonRefresher, IonRefresherContent  } from "@ionic/vue";
import ExploreContainer from "@/components/ExploreContainer.vue";
import { chevronForwardOutline } from "ionicons/icons";
export default {
  name: "Document",
  components: { ExploreContainer, IonContent, IonPage , IonRefresher , IonRefresherContent },
  setup() {
    const doRefresh = (event: CustomEvent) => {
      setTimeout(() => {
        event.target.complete();
      }, 2000);
    }
    return { chevronForwardOutline, doRefresh }

  },
};
</script>
<style>
.font-weight {
  font-weight: 700;
}

</style>