<script setup>
import { subscribe, autorun } from 'vue-meteor-tracker'
import { LinksCollection } from '/imports/api/links'

subscribe('links')
const links = autorun(() => LinksCollection.find({}).fetch()).result
</script>

<template>
  <div class="text-bold text-h6 q-mt-md">Learn Meteor!</div>
  <ul class="">
    <li
      v-for="link of links"
      :key="link._id"
    >
      <a
        :href="link.url"
        target="_blank"
      >{{ link.title }}</a>
    </li>
  </ul>
</template>
