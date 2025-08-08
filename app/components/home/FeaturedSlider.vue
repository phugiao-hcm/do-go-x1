<template>
  <section class="py-8 px-4">
    <div class="max-w-screen-xl mx-auto">
      <!-- Header -->
      <div>
        <h2 class="text-4xl font-bold text-black mb-3">SẢN PHẨM NỔI BẬT</h2>
        <p class="text-gray-500 text-lg max-w-2xl">
          Những mẫu đồ gỗ tinh tế, chất lượng cao, phù hợp với mọi không gian
          sống, mang dấu ấn riêng trong kiến trúc đã góp phần biến căn nhà trong
          mơ của khách hàng thành hiện thực.
        </p>
      </div>
      <!-- Category Tabs -->
      <div class="flex flex-wrap gap-2 my-6">
        <button
          v-for="(tab, index) in tabs"
          :key="index"
          :class="[
            'px-4 py-2 rounded font-medium',
            activeTab === tab
              ? 'bg-red-600 text-white'
              : 'bg-gray-100 text-gray-700',
          ]"
          @click="activeTab = tab"
        >
          {{ tab }}
        </button>
      </div>

      <!-- Product Grid -->
      <div
        class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-6"
      >
        <div
          v-for="(product, index) in filteredProducts"
          :key="index"
          class="border rounded-lg overflow-hidden shadow-sm hover:shadow-lg transition"
        >
          <img
            :src="product.image"
            :alt="product.title"
            class="w-full h-48 object-cover"
          />
          <div class="p-4">
            <h3 class="text-sm font-medium text-gray-800 mb-2 leading-snug">
              {{ product.title }}
            </h3>
            <p class="text-red-600 font-semibold text-lg">
              {{ product.price }} đ
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, computed } from "vue";

const tabs = [
  "Bàn ghế gỗ",
  "Tủ tivi",
  "Giường ngủ",
  "Tủ quần áo",
  "Bàn ăn",
  "Bàn - tủ thờ",
  "Bàn làm việc",
  "Ghế làm việc",
  "Gỗ mỹ nghệ",
];

const activeTab = ref("Bàn ghế gỗ");

// Fake products (replace with real API data or props)
const products = ref([
  {
    title: "Bộ bàn ghế gỗ hương đá chạm đào, tay 14, 10 món – BBG3710",
    price: "183.000.000",
    image: "images/noibat_1.png",
    category: "Bàn ghế gỗ",
  },
  {
    title: "Bộ bàn ghế triện mặt liền gỗ gõ đỏ 6 món tay 12 | BBG2121",
    price: "47.900.000",
    image: "images/noibat_2.png",
    category: "Bàn ghế gỗ",
  },
  {
    title: "Bộ bàn ghế Sofa Hoàng Gia Luxury 6 món BBG5916",
    price: "509.000.000",
    image: "images/noibat_3.png",
    category: "Bàn ghế gỗ",
  },
  {
    title: "Ghế bập bênh thư giãn gỗ gõ đỏ - GBB202",
    price: "8.600.000",
    image: "images/noibat_4.png",
    category: "Bàn ghế gỗ",
  },
  {
    title: "Ghế bập bênh thư giãn gỗ gõ đỏ - GBB202",
    price: "8.600.000",
    image: "images/noibat_5.png",
    category: "Bàn ghế gỗ",
  },
  {
    title: "Ghế bập bênh massge gỗ gỏ đỏ-GBB203",
    price: "10.600.000",
    image: "images/noibat_6.png",
    category: "Bàn ghế gỗ",
  },
  {
    title: "Sofa hiện đại gõ đỏ 5 món bọc simili BBG024",
    price: "45.900.000",
    image: "images/noibat_7.png",
    category: "Bàn ghế gỗ",
  },
  {
    title: "Ghế thư giãn massge gỗ hương đá – BBG767",
    price: "5.200.000",
    image: "images/noibat_8.png",
    category: "Bàn ghế gỗ",
  },
  {
    title: "Bộ bàn ghế hoàng gia bọc da bò Ita gõ đỏ 06 món BBG3501",
    price: "97.000.000",
    image: "images/noibat_9.png",
    category: "Bàn ghế gỗ",
  },
  {
    title: "Ghế thư giãn massge cẩm lai xịn – BBG463",
    price: "10.300.000",
    image: "images/noibat_10.png",
    category: "Bàn ghế gỗ",
  },
]);

const filteredProducts = computed(() => {
  return products.value.filter((p) => p.category === activeTab.value);
});
</script>
