<template>
  <div class="text-xl" id="app">
    姓名： {{ name }}
    年龄：
    <button @click="changeAge(-1)">-</button>
    {{ age }}
    <button @click="changeAge(1)">+</button>
  </div>
</template>

<script lang="ts">
  import { defineComponent } from 'vue';
  import { ConfigProvider } from 'ant-design-vue';

  export default defineComponent({
    name: 'App',
    components: { ConfigProvider },
    props: {
      // t: String,
    },
    setup() {
      return {};
    },
  });
</script>
