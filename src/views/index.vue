<script setup lang="ts">
  const router = useRouter()

  const name = ref('')
  function go() {
    router.push({ name: 'all', params: { all: name.value } })
  }
</script>

<template>
  <div flex="~ col items-center" class="gap-4">
    <div class="font-mono text-xs gap-2" flex="~ items-center">
      <i i-carbon:campsite class="text-2xl" />
      <span>Vite + Antdv</span>
    </div>
    <a-input v-model:value="name" placeholder="你是谁？" />
    <a-button :disabled="!name" @click="go">
      Go
    </a-button>
  </div>
</template>
