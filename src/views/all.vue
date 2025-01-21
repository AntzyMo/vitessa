<script setup lang="ts">

</script>

<template>
  <div class="mb-2">
    Hi {{ $route.params.all }}
  </div>
  <RouterLink to="/" replace>
    <a-button>
      Back
    </a-button>
  </RouterLink>
</template>
