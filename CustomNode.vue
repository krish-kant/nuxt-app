<script setup >
import { Position } from '@vue-flow/core'

// props were passed from the slot using `v-bind="customNodeProps"`
const props = defineProps(['label'])
</script>

<template>
  <div>
    <Handle type="target" :position="Position.Top" />
    <div class="" >{{ label }}</div>
    <Handle type="source" :position="Position.Bottom" />
  </div>
</template>
<!-- <style >.vue-flow__node-custom {
    background: whitesmoke;
    color: black;
    padding: 10px;
    min-width: 200px;
    font-size: small;
    border-radius: 4px;

}</style> -->