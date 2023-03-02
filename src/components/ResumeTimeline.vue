<script setup lang="ts">
import { ref } from 'vue'

const companies = ref([
  {
    label: '上海昇悦数字科技有限公司',
    date: '2021/08 - 至今',
    description: '任前端架构师，主要负责前端工具链的编写，低代码设计器和引擎的迭代。',
  },
  {
    label: '⽆锡佰东健康有限公司',
    date: '2019/03 - 2021/08',
    description: '任前端技术组组长，主要负责技术选型，前端工具链的编写，架构、规范、工作流的建立。以及应用核心模块的编写。',
  },
  {
    label: '成都海成科技有限公司',
    date: '2018/03 - 2019/02',
    description: '任中级前端开发工程师，主要负责分析需求，根据原型图使应用落地。',
  },
  {
    label: '成都和时与科技有限公司',
    date: '2016/09 - 2017/11',
    description: '任初级前端开发工程师，主要负责还原设计图，混合开发应用的编写和打包。',
  },
])
</script>

<template>
  <resume-block title="工作经历">
    <var-steps
      class="resume-timeline"
      direction="vertical"
      :active="companies.length - 1"
    >
      <var-step
        current-icon="map-marker"
        active-icon="map-marker"
        v-for="c in companies"
        :key="c.label"
      >
        <div class="resume-timeline-company">
          <div class="resume-timeline-label">{{ c.label }}</div>
          <div class="resume-timeline-date">{{ c.date }}</div>
          <div class="resume-timeline-description">{{ c.description }}</div>
        </div>
      </var-step>
    </var-steps>
  </resume-block>
</template>

<style lang="less" scoped>
.resume-timeline {
  &-company {
    margin-left: 10px;
  }

  &-label {
    font-size: 16px;
  }

  &-date {
    color: #aaa;
    margin: 6px 0;
  }

  &-description {
    color: #555;
  }
}
</style>
