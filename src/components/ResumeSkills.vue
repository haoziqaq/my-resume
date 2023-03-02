<script setup lang="ts">
import { ref } from 'vue'

const skills = ref([
  {
    label: 'Varlet UI',
    value: 100,
  },
  {
    label: 'Vant',
    value: 90,
  },
  {
    label: 'Ant Design Vue',
    value: 90,
  },
  {
    label: 'Javascript',
    value: 90,
  },
  {
    label: 'Typescript',
    value: 90,
  },
  {
    label: 'Vue',
    value: 90,
  },
  {
    label: 'HTML',
    value: 90,
  },
  {
    label: 'CSS',
    value: 80,
  },
  {
    label: 'Nodejs',
    value: 80,
  },
  {
    label: 'Vite',
    value: 80,
  },
  {
    label: 'Webpack',
    value: 80,
  },
  {
    label: 'Rollup',
    value: 70,
  },
  {
    label: 'Electron',
    value: 70,
  },
  {
    label: 'React',
    value: 70,
  },
  {
    label: 'React Native',
    value: 70,
  },
])
</script>

<template>
  <resume-block title="技能自评">
    <var-row class="resume-skills" justify="center" :gutter="20">
      <var-col
        class="resume-skills-chart"
        direction="column"
        align="center"
        v-for="s in skills"
        :key="s.label"
        :span="4"
      >
        <var-progress
          mode="circle"
          label
          line-width="5"
          :value="s.value"
          :size="75"
        >
          <span class="resume-skills-value">{{ s.value }}</span>
        </var-progress>
        <span class="resume-skills-label">{{ s.label }}</span>
      </var-col>
    </var-row>
  </resume-block>
</template>

<style lang="less" scoped>
.resume-skills {
  width: 100%;
  margin-top: 20px;

  &-paper {
    padding: 20px;
  }

  &-title {
    font-size: 18px;
    padding-bottom: 18px;
    padding-left: 2px;
    margin-bottom: 30px;
    border-bottom: thin solid #ddd;
  }

  &-label {
    margin-top: 10px;
    font-size: 16px;
    color: #666;
    text-align: center;
  }

  &-value {
    font-size: 18px;
  }

  &-chart {
    margin: 10px 0;
  }
}
</style>
