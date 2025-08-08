<template>
  <section
    class="relative bg-cover bg-center bg-no-repeat min-h-screen"
    style="background-image: url('/images/hero-wood.png')"
  >
    <!-- Overlay đen mờ -->
    <div class="absolute inset-0 bg-black/50"></div>

    <!-- Nội dung căn giữa màn hình -->
    <div
      class="relative z-10 flex flex-col items-center justify-center text-center text-white h-full px-4"
    >
      <h1 class="text-4xl md:text-5xl font-bold leading-tight drop-shadow-lg">
        Nghệ Thuật Từ Gỗ Tự Nhiên
      </h1>
      <p class="mt-4 text-lg max-w-2xl drop-shadow">
        Sản phẩm thủ công tinh xảo mang đến vẻ đẹp bền vững và sang trọng cho
        không gian sống.
      </p>
      <NuxtLink
        to="/"
        class="mt-6 bg-amber-600 hover:bg-amber-700 text-white py-3 px-6 rounded-lg transition"
      >
        Khám Phá Ngay
      </NuxtLink>
    </div>
  </section>
</template>

<style scoped>
section {
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
