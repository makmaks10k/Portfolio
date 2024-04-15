<script>
export default {
  setup() {
    return {
      bios: [
        {
          id: 1,
          bio: "Hey there! I'm Michael, a melody weaver with a penchant for pixels and a knack for capturing life's fleeting moments through the lens. When I'm not immersed in the world of composition, crafting musical landscapes that resonate with emotion, you'll find me exploring virtual realms, honing my skills as a gamer with every challenge conquered. Photography is my canvas, where I paint with light and shadow, freezing time to tell stories that words alone cannot convey. Alongside my artistic pursuits, I'm deeply passionate about programming, diving into the intricate world of code to build digital creations that push boundaries and spark innovation. As an aspiring IT student, I navigate the complex networks of code and technology with a curious mind and a thirst for knowledge. Each click of the camera shutter and each line of code written adds a new layer to the symphony of my growth, blending creativity with technical acumen in perfect harmony.",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
    <!-- About profile image -->
    <div class="w-full sm:w-1/4 mb-7 sm:mb-0">
      <img src="@/assets/images/profile.jpg" class="rounded-xl w-96" alt="" />
    </div>

    <!-- About details -->
    <div class="w-full sm:w-3/4 text-left">
      <p
        v-for="bio in bios"
        :key="bio.id"
        class="font-general-regular mb-4 text-ternary-dark dark:text-ternary-light text-lg"
      >
        {{ bio.bio }}
      </p>
    </div>
  </div>
</template>
