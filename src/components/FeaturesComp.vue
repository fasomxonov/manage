<template>
  <div
    class="flex flex-col px-4 container mx-auto mt-10 space-y-12 md:space-y-0 md:flex-row"
  >
    <div class="flex flex-col space-y-8 md:space-y-12 md:w-1/2">
      <h2
        class="text-3xl font-bold text-center md:max-w-md md:text-4xl md:text-left"
      >
        Whats different about Manage?
      </h2>
      <p class="text-center text-gray-500 md:max-w-sm md:text-left">
        Manage provides all the functionality your team needs, without the
        complexity. Our software is tailor-made for modern digital product
        teams.
      </p>
    </div>

    <div class="flex flex-col space-y-8 md:w-1/2">
      <div
        class="flex flex-col space-y-3 md:space-y-1 md:space-x-6 md:flex-row"
        v-for="manageList in manageLists"
        :key="manageList.number"
      >
        <div class="rounded-l-full bg-red-400 md:bg-transparent">
          <div class="flex items-center space-x-2">
            <div class="px-4 py-2 text-white rounded-full md:py-1 bg-red-600">
              {{ manageList.number }}
            </div>
            <h3
              class="text-base font-bold text-white md:text-black md:mb-4 md:hidden"
            >
              {{ manageList.title }}
            </h3>
          </div>
        </div>

        <div>
          <h3 class="hidden mb-4 text-lg font-bold md:block">
            {{ manageList.title }}
          </h3>
          <p class="text-gray-500">
            {{ manageList.description }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      manageLists: [
        {
          number: "01",
          title: "Track company-wide progress",
          description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Harum, sit eum? Ad odit eum et, minus esse aperiam laborum modi aliquid, aliquam, mollitia odio dicta magni tempora quas delectus sapiente.",
        },
        {
          number: "02",
          title: "Advanced built-in reports",
          description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Harum, sit eum? Ad odit eum et, minus esse aperiam laborum modi aliquid, aliquam, mollitia odio dicta magni tempora quas delectus sapiente.",
        },
        {
          number: "03",
          title: "Everything you need in one place",
          description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Harum, sit eum? Ad odit eum et, minus esse aperiam laborum modi aliquid, aliquam, mollitia odio dicta magni tempora quas delectus sapiente.",
        },
      ],
    };
  },
};
</script>
