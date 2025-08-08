<template>
  <section class="bg-white py-10 px-4">
    <div class="max-w-7xl mx-auto">
      <h2 class="text-2xl font-bold text-red-600 mb-6 uppercase">
        Danh mục sản phẩm
      </h2>
      <div
        class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-6 gap-4"
      >
        <div
          v-for="(item, index) in categories"
          :key="index"
          class="border-2 border-red-500 rounded-lg p-4 flex flex-col items-center text-center hover:shadow-lg transition"
        >
          <img
            :src="item.image"
            :alt="item.title"
            class="h-20 mb-2 object-contain"
          />
          <p class="text-sm font-medium">{{ item.title }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const categories = [
  { title: "Bàn ghế sofa", image: "images/sofa.png" },
  { title: "Tủ kệ tivi", image: "images/tu-ke-tivi.png" },
  { title: "Tranh treo tường", image: "images/tranh.png" },
  { title: "Tủ rượu", image: "images/tu-ruou.png" },
  { title: "Lục bình gỗ", image: "images/luc-binh.png" },
  { title: "Đồng hồ cây", image: "images/dong-ho-cay.png" },
  { title: "Mỹ nghệ trang trí", image: "images/my-nghe.png" },
  { title: "Giường ngủ", image: "images/giuong-ngu.png" },
  { title: "Tủ quần áo", image: "images/tu-quan-ao.png" },
  { title: "Bàn trang điểm", image: "images/ban-trang-diem.png" },
  { title: "Tủ đầu giường", image: "images/tu-dau-giuong.png" },
  { title: "Bộ bàn ăn", image: "images/bo-ban-an.png" },
  { title: "Mặt bàn nguyên tấm", image: "images/mat-ban.png" },
  { title: "Mẫu ghế ăn", image: "images/ghe-an.png" },
  { title: "Bàn trang trí", image: "images/ban-trang-tri.png" },
  { title: "Sập thờ", image: "images/sap-tho.png" },
  { title: "Bàn thờ thần tài", image: "images/ban-than-tai.png" },
  { title: "Bàn làm việc", image: "images/ban-lam-viec.png" },
  { title: "Ghế làm việc", image: "images/ghe-lam-viec.png" },
  { title: "P. khách hoàng gia", image: "images/p-khach.png" },
  { title: "Phòng ngủ hoàng gia", image: "images/p-ngu.png" },
  { title: "Phòng ăn hoàng gia", image: "images/p-an.png" },
];
</script>

<style scoped>
/* Optional custom styles */
</style>
