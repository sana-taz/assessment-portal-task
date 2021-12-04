<template>
  <div class="rounded-md">
    <header class="cursor-pointer">
      <div
        class="bg-white rounded-t-lg 2xl:px-6 xl:px-6 lg:px-6 md:px-6 px-1 pt-4 pb-4"
      >
        <ul class="flex flex-row w-full justify-center">
          <li
            v-for="tab in tabs"
            :key="tab"
            class="py-2 2xl:px-6 xl:px-6 lg:px-6 md:px-6 px-2 lg:py-2 tab-head"
            :class="{
              '  text-md font-medium text-black transition border-b-4 border-black duration-500  ease-in-out ':
                activeTab === tab,
            }"
            @click="switchTab(tab)"
          >
            <slot :name="tabHeadSlotName(tab)">{{ tab }} </slot>
          </li>
        </ul>
      </div>
    </header>
    <main
      class="bg-white card-body 2xl:p-4 xl:p-4 lg:p-4 md:p-4 p-2 rounded-b-lg"
    >
      <div class="tab-panel 2xl:px-4 xl:px-4 lg:px-4 md:px-4 px-1">
        <slot :name="tabPanelSlotName"> </slot>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  props: {
    initialTab: String,
    tabs: Array,
  },
  data() {
    return {
      activeTab: this.tabs[0],
    }
  },
  computed: {
    tabPanelSlotName() {
      return `tab-panel-${this.activeTab}`
    },
  },
  watch: {
    initialTab(value) {
      this.activeTab = this.tabs[this.tabs.indexOf(value)]
    },
  },
  methods: {
    tabHeadSlotName(tabName) {
      return `tab-head-${tabName}`
    },

    switchTab(tabName) {
      this.activeTab = tabName
      this.$emit('activetab', tabName)
    },
  },
}
</script>

<style scoped>
/* .card-body {
  padding: 20px 16px;
} */
</style>
