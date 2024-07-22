<script setup>
import { ref } from 'vue'
import {
  QBtn,
  QCard,
  QIcon,
  QCardSection
} from 'quasar'
const count = ref(0)

function increment() {
  count.value++
}
</script>

<template>
  <QCard class="bg-tertiary">
    <QCardSection>
      <p>
        You've pressed the button <strong>{{ count }}</strong> times.
      </p>
      <QBtn
        @click="increment"
        color="primary"
      >
        <QIcon
          name="fas fa-plus"
          size="1em"
          class="q-mr-sm"
        />
        Qbtn with Fontawesome icon
      </QBtn>
    </QCardSection>
  </QCard>
</template>
