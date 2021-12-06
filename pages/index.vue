<template>
  <div class="flex w-full h-screen">
    <div class="flex flex-col w-full h-full">
      <div class="flex shadow-2xl w-full justify-start">
        <header class="flex p-8 text-sm">LOGO</header>
      </div>
      <div class="flex w-full justify-center mt-12">
        <div class="text-sm container p-4 bg-gray-200 m-4">
          Lorem Ipsum is simply dummy text of the printing and typesetting
          industry. Lorem Ipsum has been the industry's standard dummy text ever
          since the 1500s, when an unknown printer took a galley of type and
          scrambled it to make a type specimen book. It has survived not only
          five centuries, but also the leap into electronic typesetting,
          remaining essentially unchanged. It was popularised in the 1960s with
          the release of Letraset sheets containing Lorem Ipsum passages, and
          more recently with desktop publishing software like Aldus PageMaker
          including versions of Lorem Ipsum. Lorem Ipsum is simply dummy text of
          the printing and typesetting industry. Lorem Ipsum has been the
          industry's standard dummy text ever since the 1500s, when an unknown
          printer took a galley of type and scrambled it to make a type specimen
          book. It has survived not only five centuries, but also the leap into
          electronic typesetting, remaining essentially unchanged. It was
          popularised in the 1960s with the release of Letraset sheets
          containing Lorem Ipsum passages, and more recently with desktop
          publishing software like Aldus PageMaker including versions of Lorem
          Ipsum. Lorem Ipsum is simply dummy text of the printing and
          typesetting industry. Lorem Ipsum has been the industry's standard
          dummy text ever since the 1500s, when an unknown printer took a galley
          of type and scrambled it to make a type specimen book. It has survived
          not only five centuries, but also the leap into electronic
          typesetting, remaining essentially unchanged. It was popularised in
          the 1960s with the release of Letraset sheets containing Lorem Ipsum
          passages, and more recently with desktop publishing software like
          Aldus PageMaker including versions of Lorem Ipsum. Lorem Ipsum is
          simply dummy text of the printing and typesetting industry. Lorem
          Ipsum has been the industry's standard dummy text ever since the
          1500s, when an unknown printer took a galley of type and scrambled it
          to make a type specimen book. It has survived not only five centuries,
          but also the leap into electronic typesetting, remaining essentially
          unchanged. It was popularised in the 1960s with the release of
          Letraset sheets containing Lorem Ipsum passages, and more recently
          with desktop publishing software like Aldus PageMaker including
          versions of Lorem Ipsum.
        </div>
      </div>
      <div class="flex w-full justify-center">
        <div>
          <Tab
            :tabs="tabs"
            :initial-tab="initialTab"
            @activetab="settab($event)"
          >
            <template
              slot="tab-head-General Question"
              class="font-medium text-gray-500 border-b-2 border-blue-600"
            >
              General Question
            </template>
            <template slot="tab-panel-General Question">
              <div class="flex flex-col w-full justify-start">
                <div class="text-sm my-2 font-bold">
                  1. This is a question that needs to be answered
                </div>
                <div class="flex w-full mt-2 mb-6">
                  <textarea
                    class="bg-gray-100 hover:bg-gray-200 focus:outline-none focus:bg-gray-200 flex w-full"
                    rows="5"
                    cols="100%"
                  ></textarea>
                </div>
                <div class="text-sm my-2 font-bold">
                  2. This is a question that needs to be answered
                </div>
                <div class="flex w-full mt-2 mb-6">
                  <textarea
                    class="bg-gray-100 hover:bg-gray-200 focus:outline-none focus:bg-gray-200 flex w-full"
                    rows="5"
                    cols="100%"
                  ></textarea>
                </div>
                <div class="text-sm my-2 font-bold">
                  3. This is a question that needs to be answered
                </div>
                <div class="flex w-full mt-2 mb-6">
                  <textarea
                    class="bg-gray-100 hover:bg-gray-200 focus:outline-none focus:bg-gray-200 flex w-full"
                    rows="5"
                    cols="100%"
                  ></textarea>
                </div>
              </div>
              <div class="flex justify-end w-full mt-6">
                <button
                  class="bg-gray-300 hover:bg-gray-400 px-4 py-2 rounded-md"
                  @click="settab('Personality Assessment')"
                >
                  Go to Personality assessment
                </button>
              </div>
            </template>
            <template
              slot="tab-head-Personality Assessment"
              class="font-medium text-gray-500 border-b-2 border-blue-600"
            >
              Personality Assessment
            </template>
            <template slot="tab-panel-Personality Assessment">
              <div class="flex flex-col w-full justify-center">
                <div class="text-sm my-2 font-bold">
                  The personality assessment contains 12 sections with 10
                  questions each. Please do not overthink. The answers to the
                  questions is done on scale.
                </div>
                <div class="flex justify-center w-full">
                  <div
                    class="flex flex-row justify-evenly 2xl:w-3/4 xl:w-3/4 lg:3/4 md:w-full w-full mt-2 mb-6"
                  >
                    <div
                      class="bg-red-400 w-1/5 py-6 2xl:mx-4 xl:mx-4 lg:mx-4 md:mx-4 mx-1 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                    >
                      <div class="text-center sm:text-sm text-xs">
                        Strongly Disagree
                      </div>
                    </div>
                    <div
                      class="bg-red-200 w-1/5 py-6 2xl:mx-4 xl:mx-4 lg:mx-4 md:mx-4 mx-1 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                    >
                      <div class="text-center sm:text-sm text-xs">Disagree</div>
                    </div>
                    <div
                      class="bg-gray-400 w-1/5 py-6 2xl:mx-4 xl:mx-4 lg:mx-4 md:mx-4 mx-1 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                    >
                      <div class="text-center sm:text-sm text-xs">Neutral</div>
                    </div>
                    <div
                      class="bg-green-200 w-1/5 py-6 2xl:mx-4 xl:mx-4 lg:mx-4 md:mx-4 mx-1 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                    >
                      <div class="text-center sm:text-sm text-xs">Agree</div>
                    </div>
                    <div
                      class="bg-green-500 w-1/5 py-6 2xl:mx-4 xl:mx-4 lg:mx-4 md:mx-4 mx-1 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                    >
                      <div class="text-center sm:text-sm text-xs">
                        Strongly Agree
                      </div>
                    </div>
                  </div>
                </div>
                <div class="text-sm my-2 font-bold">
                  1. This is a question that needs to be answered
                </div>
                <div
                  class="flex flex-row 2xl:w-3/4 xl:w-3/4 lg:3/4 md:w-3/4 w-full mb-4"
                >
                  <div
                    class="bg-red-400 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="stronglyDisagreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="stonglydisagreed"
                    />
                  </div>
                  <div
                    class="bg-red-200 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="disagreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="disagreed"
                    />
                  </div>
                  <div
                    class="bg-gray-400 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="neutralId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="neutral"
                    />
                  </div>
                  <div
                    class="bg-green-200 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="agreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="agree"
                    />
                  </div>
                  <div
                    class="bg-green-500 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="stronglyAgreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="agree"
                    />
                  </div>
                </div>
                <div class="text-sm my-2 font-bold">
                  2. This is a question that needs to be answered
                </div>
                <div
                  class="flex flex-row 2xl:w-3/4 xl:w-3/4 lg:3/4 md:w-3/4 w-full mb-4"
                >
                  <div
                    class="bg-red-400 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="stronglyDisagreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="stonglydisagreed"
                    />
                  </div>
                  <div
                    class="bg-red-200 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="disagreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="disagreed"
                    />
                  </div>
                  <div
                    class="bg-gray-400 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="neutralId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="neutral"
                    />
                  </div>
                  <div
                    class="bg-green-200 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="agreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="agree"
                    />
                  </div>
                  <div
                    class="bg-green-500 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="stronglyAgreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="agree"
                    />
                  </div>
                </div>
                <div class="text-sm my-2 font-bold">
                  3. This is a question that needs to be answered
                </div>
                <div
                  class="flex flex-row 2xl:w-3/4 xl:w-3/4 lg:3/4 md:w-3/4 w-full mb-4"
                >
                  <div
                    class="bg-red-400 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="stronglyDisagreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="stonglydisagreed"
                    />
                  </div>
                  <div
                    class="bg-red-200 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="disagreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="disagreed"
                    />
                  </div>
                  <div
                    class="bg-gray-400 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="neutralId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="neutral"
                    />
                  </div>
                  <div
                    class="bg-green-200 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="agreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="agree"
                    />
                  </div>
                  <div
                    class="bg-green-500 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="stronglyAgreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="agree"
                    />
                  </div>
                </div>
                <div class="text-sm my-2 font-bold">
                  4. This is a question that needs to be answered
                </div>
                <div
                  class="flex flex-row 2xl:w-3/4 xl:w-3/4 lg:3/4 md:w-3/4 w-full mb-4"
                >
                  <div
                    class="bg-red-400 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="stronglyDisagreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="stonglydisagreed"
                    />
                  </div>
                  <div
                    class="bg-red-200 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="disagreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="disagreed"
                    />
                  </div>
                  <div
                    class="bg-gray-400 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="neutralId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="neutral"
                    />
                  </div>
                  <div
                    class="bg-green-200 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="agreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="agree"
                    />
                  </div>
                  <div
                    class="bg-green-500 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="stronglyAgreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="agree"
                    />
                  </div>
                </div>
                <div class="text-sm my-2 font-bold">
                  5. This is a question that needs to be answered
                </div>
                <div
                  class="flex flex-row 2xl:w-3/4 xl:w-3/4 lg:3/4 md:w-3/4 w-full mb-4"
                >
                  <div
                    class="bg-red-400 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="stronglyDisagreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="stonglydisagreed"
                    />
                  </div>
                  <div
                    class="bg-red-200 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="disagreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="disagreed"
                    />
                  </div>
                  <div
                    class="bg-gray-400 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="neutralId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="neutral"
                    />
                  </div>
                  <div
                    class="bg-green-200 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="agreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="agree"
                    />
                  </div>
                  <div
                    class="bg-green-500 transition transform hover:-translate-y-1 motion-reduce:transition-none motion-reduce:transform-none w-1/5 py-6 mx-2 2xl:h-20 xl:h-20 lg:h-20 md:h-20 h-14 flex justify-center items-center rounded text-white"
                  >
                    <input
                      id="stronglyAgreeId"
                      class="hidden"
                      type="radio"
                      name="answer"
                      value="agree"
                    />
                  </div>
                </div>
              </div>
              <div class="flex justify-end w-full mt-6">
                <button
                  class="bg-gray-300 hover:bg-gray-400 px-4 py-2 rounded-md"
                  @click="settab(nextTab)"
                >
                  Next Section
                </button>
              </div>
            </template>
          </Tab>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Tab from '~/components/Tab'

export default {
  name: 'App',
  components: {
    Tab,
  },
  data() {
    return {
      initialTab: 'General Question',
      lastTab: 'Personality Assessment',
      tabs: ['General Question', 'Personality Assessment'],
    }
  },
  computed: {
    nextTab() {
      return this.tabs[this.tabs.length - 1]
    },
  },
  watch: {
    $route() {},
  },
  methods: {
    settab(tab) {
      console.log(tab)
      this.initialTab = tab
    },
    onClick() {
      // console.log(this.initialTab)
      // this.initialTab = 'Personality Assessment'
      // console.log(this.initialTab)
      // return (this.initialTab = 'Personality Assessment')
      // const routeData = this.$router.resolve({
      //   name: 'routeName',
      //   query: { data: 'someData' },
      // })
      // window.open(routeData.href, '_blank')
      // return this.$router.push({ path: this.lastTab })
    },
  },
}
</script>
