<template>
  <app-layout title="Settings">
    <base-renderer title="Tray Icon" :settings="settings"></base-renderer>
  </app-layout>
</template>

<script>
import AppLayout from '@layouts/AppLayout';
import SettingsMixin from '@mixins/SettingsMixin';
import BaseRenderer from './BaseRenderer';

export default {
  components: {
    AppLayout,
    BaseRenderer,
  },

  mixins: [SettingsMixin],

  data() {
    return {
      group: 'trayIcon',
    }
  },
}
</script>
