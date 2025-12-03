<template>
  <div>
    <p>attrs.msg: {{ attrs.msg }}</p>
    <p>watchEffect 触发次数: {{ count }}</p>
  </div>
</template>

<script setup>
import { useAttrs, watchEffect, ref } from 'vue'

const attrs = useAttrs()
const count = ref(0)

// 用 watchEffect 证明读取 attrs 会收集依赖
watchEffect(() => {
  // 读取 attrs.msg 会触发 track
  console.log('读取 attrs.msg:', attrs.msg)
  count.value++ // 每次依赖触发都会执行
})
</script>