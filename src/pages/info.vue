<template>
  <div class="p-8">
    <figure class="xl:flex bg-gray-100 rounded-xl p-8 shadow-md">
      <img
        class="w-32 h-32 rounded-full mx-auto"
        src="../assets/profile1.jpg"
      />
      <div class="pt-6 text-center space-y-4">
        <blockquote>
          <p class="text-lg font-semibold">
            {{ name }} {{ surname }} ({{ age }})
          </p>
        </blockquote>
        <figcaption class="font-medium">
          <div class="text-cyan-600">{{ university }}</div>
          <div class="break-words text-gray-500">
            <span v-for="skill in skills" :key="skill">
              {{ skill }}
              <span v-if="skill != skills[skills.length - 1]">, </span>
            </span>
          </div>
          <div class="pt-6">
            <router-link :to="{ name: 'contact' }">
              <a class="text-gray-500 hover:text-yellow-500">
                <strong>contact ></strong>
              </a>
            </router-link>
          </div>
        </figcaption>
      </div>
    </figure>
  </div>
</template>

<script>
export default {
  data: () => ({
    name: "Methichai",
    surname: "Preedanorawut",
    age: 21,
    university: "Thai-Nichi Institute of Technology",
    skills: ["Python", "JS", "HTML", "CSS", "SQL"],
  }),
};
</script>