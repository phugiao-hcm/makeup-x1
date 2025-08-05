<template>
    <section class="py-16 bg-white">
        <div class="max-w-7xl mx-auto px-4">
            <!-- Tiêu đề -->
            <div class="text-center mb-12">
                <h2 class="text-3xl md:text-4xl font-bold text-purple-700">
                    Mẫu Makeup
                </h2>
                <div class="mt-2 w-16 h-1 bg-purple-700 mx-auto"></div>
            </div>

            <!-- Danh sách sản phẩm -->
            <div
                class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-8"
            >
                <div
                    v-for="(item, index) in products"
                    :key="index"
                    class="text-center space-y-2"
                >
                    <!-- Ảnh sản phẩm -->
                    <img
                        :src="item.image"
                        :alt="item.title"
                        class="w-full rounded-md shadow-md"
                    />

                    <!-- Thể loại -->
                    <p class="text-sm text-gray-500">Mẫu Makeup</p>

                    <!-- Tiêu đề -->
                    <h3 class="text-base font-semibold text-purple-600">
                        {{ item.title }}
                    </h3>

                    <!-- Rating -->
                    <div class="text-yellow-400 text-sm">
                        <span v-for="i in 5" :key="i">
                            <i
                                class="fas"
                                :class="
                                    i <= item.rating
                                        ? 'fa-star'
                                        : 'fa-star-half-alt text-gray-300'
                                "
                            ></i>
                        </span>
                    </div>

                    <!-- Giá -->
                    <div class="text-black font-bold text-sm">
                        {{ item.price }}₫
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
const products = [
    {
        title: "TRANG ĐIỂM CHUYÊN NGHIỆP (CÔ DÂU, DẠ HỘI, DỰ TIỆC, THỜI TRANG XU HƯỚNG HIỆN ĐẠI)",
        image: "images/mau_1.png",
        rating: 5,
        price: "25.000",
    },
    {
        title: "KỸ THUẬT TRANG ĐIỂM CÔ DÂU VÀ NGƯỜI MẪU THỜI TRANG (CHUYÊN NGHIỆP)",
        image: "images/mau_2.png",
        rating: 5,
        price: "25.000",
    },
    {
        title: "Lớp mới: TRANG ĐIỂM PHONG CÁCH THỜI THƯỢNG",
        image: "images/mau_3.png",
        rating: 2,
        price: "25.000",
    },
    {
        title: "TRANG ĐIỂM ỨNG DỤNG XU HƯỚNG MỚI (HOT TREND)",
        image: "images/mau_4.png",
        rating: 2,
        price: "25.000",
    },
    {
        title: "TRANG ĐIỂM THẨM MỸ",
        image: "images/mau_5.png",
        rating: 2,
        price: "25.000",
    },
    {
        title: "TRANG ĐIỂM CHUYÊN SÂU",
        image: "images/mau_6.png",
        rating: 2,
        price: "25.000",
    },
];
</script>

<style scoped>
@import url("https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css");
</style>
