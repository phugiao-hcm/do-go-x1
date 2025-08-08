<template>
  <section class="bg-white py-16 px-6">
    <div
      class="max-w-screen-xl mx-auto flex flex-col lg:flex-row items-center gap-10"
    >
      <!-- Left content -->
      <div class="lg:w-1/2">
        <h2 class="text-4xl font-extrabold text-black mb-4">
          Quy trình sản xuất
        </h2>
        <p class="text-gray-600 mb-8">
          Chúng tôi cam kết mang đến những sản phẩm đồ gỗ chất lượng cao, được
          thực hiện tỉ mỉ qua từng công đoạn. Từ khâu tư vấn, thiết kế đến sản
          xuất và giao hàng, mọi quy trình đều được kiểm soát chặt chẽ để đảm
          bảo sự hài lòng của khách hàng.
        </p>

        <!-- Steps -->
        <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
          <!-- Step 1 -->
          <div
            class="bg-gradient-to-br from-orange-400 to-orange-600 text-white p-6 rounded-xl shadow-md relative"
          >
            <h3 class="text-xl font-bold mb-2">Tư Vấn & Đặt Hàng</h3>
            <p class="text-sm">
              Đội ngũ tư vấn hỗ trợ khách hàng lựa chọn sản phẩm phù hợp với nhu
              cầu và không gian sử dụng. Có thể đặt theo mẫu có sẵn hoặc thiết
              kế theo yêu cầu.
            </p>
            <span
              class="absolute top-4 right-4 text-4xl font-extrabold opacity-20"
              >1</span
            >
          </div>

          <!-- Step 2 -->
          <div class="bg-white p-6 rounded-xl shadow-md relative">
            <h3 class="text-xl font-semibold text-gray-800 mb-2">
              Thiết Kế & Duyệt Mẫu
            </h3>
            <p class="text-sm text-gray-600">
              Sau khi tiếp nhận yêu cầu, đội ngũ kỹ thuật tiến hành thiết kế bản
              vẽ 3D chi tiết. Khách hàng sẽ được xem và duyệt mẫu trước khi sản
              xuất.
            </p>
            <span
              class="absolute top-4 right-4 text-4xl font-extrabold text-orange-100"
              >2</span
            >
          </div>

          <!-- Step 3 -->
          <div class="bg-white p-6 rounded-xl shadow-md relative">
            <h3 class="text-xl font-semibold text-gray-800 mb-2">
              Sản Xuất Thủ Công
            </h3>
            <p class="text-sm text-gray-600">
              Sản phẩm được gia công tại xưởng bằng gỗ tự nhiên chất lượng cao.
              Quy trình sản xuất tuân thủ tiêu chuẩn kỹ thuật, đảm bảo độ bền và
              tính thẩm mỹ.
            </p>
            <span
              class="absolute top-4 right-4 text-4xl font-extrabold text-orange-100"
              >3</span
            >
          </div>

          <!-- Step 4 -->
          <div class="bg-white p-6 rounded-xl shadow-md relative">
            <h3 class="text-xl font-semibold text-gray-800 mb-2">
              Giao Hàng & Hậu Mãi
            </h3>
            <p class="text-sm text-gray-600">
              Sản phẩm được đóng gói cẩn thận và vận chuyển tận nơi. Chúng tôi
              hỗ trợ lắp đặt và bảo hành dài hạn, đảm bảo khách hàng an tâm sử
              dụng.
            </p>
            <span
              class="absolute top-4 right-4 text-4xl font-extrabold text-orange-100"
              >4</span
            >
          </div>
        </div>
      </div>

      <!-- Right content: Triangle image -->
      <div class="lg:w-1/2 flex justify-center relative w-full">
        <svg viewBox="0 0 100 100" class="w-[300px] md:w-[400px] h-auto">
          <defs>
            <clipPath id="triangleClip">
              <polygon points="50,0 100,100 0,100" />
            </clipPath>
          </defs>

          <image
            xlink:href="/images/avt_1.png"
            width="100"
            height="100"
            preserveAspectRatio="xMidYMid slice"
            clip-path="url(#triangleClip)"
          />

          <!-- Orange triangle stroke -->
          <polygon
            points="50,0 100,100 0,100"
            fill="none"
            stroke="orange"
            stroke-width="5"
          />
        </svg>
      </div>
    </div>
  </section>
</template>


<script setup>
// No JS needed for this component
</script>

<style scoped>
</style>
