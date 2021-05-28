<template>
  <div class="p-8">
    <figure class="bg-gray-100 rounded-xl p-8 shadow-md">
      <img
        class="w-32 h-32 rounded-full mx-auto"
        src="../assets/profile2.jpg"
      />
      <div class="pt-6 text-center space-y-4">
        <figcaption class="font-medium">
          <div class="text-gray-500 text-center">
            <li>tel : {{ tel }}</li>
            <li>email : {{ email }}</li>
            <li>facebook : {{ facebook }}</li>
          </div>
        </figcaption>
      </div>
    </figure>
  </div>
</template>

<script>
export default {
  data: () => ({
    email: "peach.14975@gmail.com",
    facebook: "Peach Gsw",
    tel: "0800436798",
  }),
};
</script>