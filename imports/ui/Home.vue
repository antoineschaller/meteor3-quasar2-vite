<script setup>
import Hello from './Hello.vue'
import Info from './Info.vue'
import {
  QIcon,
} from 'quasar'
</script>

<template>
  <div class="q-pa-md">
    <div class="text-h4 text-bold q-mb-md">Welcome to Meteor</div>
    <div
      rounded
      class="bg-secondary text-white rounded-borders q-pa-md"
    >
      <div>
        <QIcon
          name="fas fa-check"
          size="1em"
        /> Meteor 3 (Full stack JavaScript framework)
      </div>
      <div>
        <QIcon
          name="fas fa-check"
          size="1em"
        /> Vue 3 (JavaScript framework)
      </div>
      <div>
        <QIcon
          name="fas fa-check"
          size="1em"
        /> Vite (Build tool)
      </div>
      <div>
        <QIcon
          name="fas fa-check"
          size="1em"
        /> Quasar 2 (UI framework)
      </div>
      <div>
        <QIcon
          name="fas fa-check"
          size="1em"
        /> Fontawesome 6 (Icon library)
      </div>
    </div>
    <Hello class="q-mt-md" />
    <Info />
  </div>
</template>
