<template>
  <div class="home">
    <ViewHeader msg="This is home page"/>
  </div>
</template>

<script>
// @ is an alias to /src
import ViewHeader from '@/components/ViewHeader.vue';

export default {
  name: 'Home',
  components: {
    ViewHeader,
  },
};
</script>
