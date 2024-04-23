<template>
  <ion-list>
    <ion-item>
      <ion-icon aria-hidden="true" :icon="airplane" slot="start"></ion-icon>
      <ion-label>Airplane Mode</ion-label>
    </ion-item>
    <ion-item>
      <ion-icon aria-hidden="true" :icon="wifi" slot="start"></ion-icon>
      <ion-label>Wi-Fi</ion-label>
    </ion-item>
    <ion-item>
      <ion-icon aria-hidden="true" :icon="bluetooth" slot="start"></ion-icon>
      <ion-label>Bluetooth</ion-label>
    </ion-item>
    <ion-item>
      <ion-icon aria-hidden="true" :icon="call" slot="start"></ion-icon>
      <ion-label>Cellular</ion-label>
    </ion-item>
  </ion-list>

  <ion-list>
    <ion-item>
      <ion-avatar aria-hidden="true" slot="start">
        <img alt="" src="https://ionicframework.com/docs/img/demos/avatar.svg" />
      </ion-avatar>
      <ion-label>Huey</ion-label>
    </ion-item>
    <ion-item>
      <ion-avatar aria-hidden="true" slot="start">
        <img alt="" src="https://ionicframework.com/docs/img/demos/avatar.svg" />
      </ion-avatar>
      <ion-label>Dewey</ion-label>
    </ion-item>
    <ion-item>
      <ion-avatar aria-hidden="true" slot="start">
        <img alt="" src="https://ionicframework.com/docs/img/demos/avatar.svg" />
      </ion-avatar>
      <ion-label>Louie</ion-label>
    </ion-item>
    <ion-item>
      <ion-avatar aria-hidden="true" slot="start">
        <img alt="" src="https://ionicframework.com/docs/img/demos/avatar.svg" />
      </ion-avatar>
      <ion-label>Fooie</ion-label>
    </ion-item>
  </ion-list>
</template>

<script lang="ts">
  import { IonAvatar, IonItem, IonLabel, IonList, IonIcon } from '@ionic/vue';
  import { defineComponent } from 'vue';
  import { airplane, bluetooth, call, wifi } from 'ionicons/icons';

  export default defineComponent({
    components: {
      IonAvatar,
      IonItem,
      IonLabel,
      IonList,
      IonIcon,
    },
    setup() {
      return { airplane, bluetooth, call, wifi };
    },
  });
</script>
<script setup lang="ts">
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar } from '@ionic/vue';
</script>

<style scoped>
#container {
  text-align: center;
  
  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

#container strong {
  font-size: 20px;
  line-height: 26px;
}

#container p {
  font-size: 16px;
  line-height: 22px;
  
  color: #8c8c8c;
  
  margin: 0;
}

#container a {
  text-decoration: none;
}
</style>
