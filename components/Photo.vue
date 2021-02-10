<template>
  <v-card rounded="xl"
              height="40%"
              width="80%"
              class="card2">
              <v-img :src="url"></v-img>
    <!-- {{ thumbnailUrl }} -->
  </v-card>
</template>

<script>
export default {
  name: 'photo',
  props:['id', 'url']

}
</script>

<style>

</style>
