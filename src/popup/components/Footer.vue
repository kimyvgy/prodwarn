<template>
  <el-footer height="50px" class="flex items-center justify-between text-xs text-gray-700">
    <a target="_blank" href="https://github.com/kimyvgy/prodwarn" class="hover:text-blue-600">
      <i class="el-icon-star-on" />
      <span>Star on Github</span>
    </a>
    <span>Prodwarn v{{ packageVersion }}</span>
  </el-footer>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Footer extends Vue {
  packageVersion = process.env.PACKAGE_VERSION;
}
</script>
