<template>
  <div class="alert border-l-4 p-4 mb-4 mt-4" :class="`alert-error`">
    <div class="flex items-start leading-7">
      <div class="flex-shrink-0 self-start pt-1">
        <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-alert-circle" width="36" height="36" viewBox="0 0 24 24" stroke-width="1.5" stroke="#2c3e50" fill="none" stroke-linecap="round" stroke-linejoin="round">
          <path stroke="none" d="M0 0h24v24H0z"/>
          <circle cx="12" cy="12" r="9" />
          <line x1="12" y1="8" x2="12" y2="12" />
          <line x1="12" y1="16" x2="12.01" y2="16" />
        </svg>
      </div>
      <div class="ml-2 alert-content">
        <slot />
      </div>
    </div>
  </div>
</template>

<script>
export default {
}
</script>

<style>
.alert p {
  @apply m-0 !important;
}
.alert a {
  @apply text-gray-700 !important;
}
.alert strong {
  @apply text-current;
}
.alert-error {
  @apply bg-red-100 border-red-400;
}
.alert-error code {
  @apply bg-red-200 shadow-none border-0 text-current;
}
.alert-error .alert-icon {
  @apply text-red-400;
}
.alert-error .alert-content {
  @apply text-red-700;
}
.dark-mode .alert a {
  @apply text-white !important;
}
.dark-mode .alert-error {
  @apply bg-yellow-900 border-yellow-700;
}
.dark-mode .alert-error .alert-content {
  @apply text-red-300 bg-yellow-900 border-yellow-700;
}
.dark-mode .alert-error .alert-content code {
  @apply bg-yellow-800 !important;
}
</style>
