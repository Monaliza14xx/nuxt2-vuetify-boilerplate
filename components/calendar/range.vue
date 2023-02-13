<template>
  <div>
    <center>
      <vc-date-picker
        class="my-6"
        v-model="range"
        is-range
        :model-config="modelConfig"
        :min-date="minDate"
        :max-date="new Date()"
        color="teal"
      >
      </vc-date-picker>
    </center>
  </div>
</template>

<script>
export default {
    data: () => ({
        range: [],
        minDate: new Date(2019, 0, 1),
        modelConfig: {
            type: 'string',
            format: 'YYYY-MM-DD',
        },
    }),
}
</script>

<style>
</style>