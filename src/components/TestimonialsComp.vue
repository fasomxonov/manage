<template>
  <div class="max-w-6xl px-5 container mx-auto mt-32 text-center">
    <h2 class="text-4xl font-bold text-center">
      What's Different About Manage?
    </h2>
    <div
      class="flex flex-col mt-24 space-y-16 md:space-y-0 md:flex-row md:space-x-6"
    >
      <div
        v-for="user in users"
        :key="user.name"
        class="flex flex-col items-center p-6 space-y-6 rounded-lg bg-gray-100 md:w-1/3"
      >
        <img
          class="w-16 -mt-14"
          src="@/assets/img/avatar-anisha.png"
          :alt="user.name"
        />
        <h5 class="text-lg font-bold">{{ user.name }}</h5>
        <p class="text-sm text-gray-500">{{ user.userInfo }}</p>
      </div>
    </div>
    <div class="my-16">
      <a
        class="p-3 px-6 pt-2 text-white bg-red-500 hover:bg-red-600 hover:shadow-xl rounded-full self-baseline transition duration-150 ease-in-out"
        href="#"
        >Get Started</a
      >
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      users: [
        {
          name: "Anisha Li",
          userInfo:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestiae aliquid ab maiores placeat in natus nobis quibusdam modi quis architecto.",
        },
        {
          name: "Anisha Li",
          userInfo:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestiae aliquid ab maiores placeat in natus nobis quibusdam modi quis architecto.",
        },
        {
          name: "Anisha Li",
          userInfo:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestiae aliquid ab maiores placeat in natus nobis quibusdam modi quis architecto.",
        },
      ],
    };
  },
};
</script>
