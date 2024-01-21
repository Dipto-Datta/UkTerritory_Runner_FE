<template>
  <div class="z-10">
    <div
      class="h-[100px] w-full bg-gray-100 grid grid-cols-7 items-center text-black px-5"
    >
      <div class="">Territory Runner TM</div>
      <div class="flex gap-2 items-center justify-center col-span-5">
        <input
          type="text"
          placeholder="Location Search"
          class="h-9 p-3 border-1 border-black rounded-lg"
        />
        <dropdown title="Contains"></dropdown>
        <checkbox
          name="Place"
          idCheckbox="Place"
          forCheckbox="Place"
        ></checkbox>
        <checkbox name="Data"></checkbox>
        <checkbox name="Layer"></checkbox>
        <checkbox name="Territory"></checkbox>
        <button class="bg-buttonColor rounded-lg py-2 px-3 text-white">
          Search
        </button>
        <button class="bg-buttonColor rounded-lg py-2 px-3 text-white">
          Reset
        </button>
        <div class="border-l-2 border-gray-600 pl-3 space-x-2">
          <button class="bg-buttonColor rounded-lg py-2 px-3 text-white">
            Demographics
          </button>
          <button class="bg-buttonColor rounded-lg py-2 px-3 text-white">
            Re-Set
          </button>
        </div>
      </div>
      <div class="flex justify-end">
        <div class="bg-green-600 rounded-lg py-2 px-3 w-3/5 text-white">
          User Name
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { ref } from "vue";
import checkbox from "@/components/widget/checkboxView.vue";
import dropdown from "@/components/widget/dropdownView.vue";
export default {
  components: {
    checkbox,
    dropdown,
  },
};
</script>
