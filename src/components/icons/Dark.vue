<template>
  <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
    <path
      d="M15.1946 15.8217C16.9231 16.1748 18.7172 16.0122 20.354 15.354C19.684 17.0213 18.5303 18.45 17.0415 19.4562C15.5527 20.4624 13.7969 21.0001 12 21C9.91037 20.9977 7.88662 20.2687 6.27565 18.9378C4.66467 17.6069 3.56683 15.757 3.17031 13.7054C2.77378 11.6537 3.10328 9.52805 4.10232 7.69272C5.10135 5.85739 6.7077 4.42673 8.64599 3.646C7.98779 5.28277 7.82514 7.0769 8.17827 8.80535C8.53139 10.5338 9.38472 12.1204 10.6322 13.3678C11.8796 14.6153 13.4662 15.4686 15.1946 15.8217Z"
      :stroke="color"
      stroke-width="2"
      stroke-linecap="round"
      stroke-linejoin="round"
    />
  </svg>
</template>

<script setup lang="ts">
type Props = {
  color?: string
}

withDefaults(defineProps<Props>(), {
  color: 'white',
})
</script>
