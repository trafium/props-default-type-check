<script lang="ts">
  import { defineComponent, PropType } from 'vue';

  type User = {
    name : string;
  }

  export default defineComponent({
    props: {
      user: {
        type: Object as PropType<User>,
        default: () => '123',
      },
    },

    setup (props) {
      console.log(props.user);
    },
  });
</script>

<template>
  <div>Hello, world</div>
</template>
