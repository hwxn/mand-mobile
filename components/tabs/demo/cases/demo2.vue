<template>
  <div class="md-example-child md-example-child-tabs md-example-child-tabs-2">
    <md-tabs
      :titles="titles"
      :default-index="2"
      show-ink-bar
    >
      <div v-for="(title, index) of titles" :key="index">
        {{title}}的内容
      </div>
    </md-tabs>
  </div>
</template>

<script>import {Tabs} from 'mand-mobile'

export default {
  name: 'tab-bar-demo',
  /* DELETE */
  title: '指定默认标签',
  titleEnUS: 'Specify the default tab',
  describe: '默认标签2',
  describeEnUS: 'Default tab 2',
  /* DELETE */
  components: {
    [Tabs.name]: Tabs,
  },
  data() {
    return {
      titles: ['第一', '第二', '第三', '第四'],
    }
  },
}
</script>