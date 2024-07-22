<script>
import {
  QToolbar,
  QBtn,
  QAvatar,
  QSpace
} from 'quasar'
</script>

<template>
  <QToolbar class="bg-primary text-white">
    <QBtn
      flat
      round
      dense
      icon="menu"
      class="q-mr-sm"
    />
    <QBtn
      flat
      :to="{ name: 'home' }"
      label="Home"
    />
    <QSpace />


    <QAvatar>
      <img src="https://cdn.quasar.dev/logo-v2/svg/logo-mono-white.svg">
    </QAvatar>
  </QToolbar>
</template>