<script setup lang="ts">
import { getEvents } from "~/lib";
const events = await getEvents();
</script>

<template>
  <div>
    <div>
      <router-link
        style="display: block"
        v-for="event in events"
        :to="'/events/' + event.slug"
        >{{ event.slug }}
      </router-link>
    </div>
  </div>
</template>
