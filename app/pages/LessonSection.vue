<template>
    <section class="bg-white py-12 px-4">
        <div class="max-w-7xl mx-auto">
            <!-- Title -->
            <div class="text-center mb-10">
                <h2 class="text-3xl font-bold text-purple-700 uppercase">
                    Danh Sách Khoá Học
                </h2>
                <div class="mt-2 text-yellow-500 text-xl">━━❥━━</div>
            </div>

            <!-- Cards -->
            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
                <div
                    v-for="(course, index) in courses"
                    :key="index"
                    class="bg-white shadow-lg rounded-lg overflow-hidden border"
                >
                    <div class="relative">
                        <img
                            :src="course.image"
                            :alt="course.title"
                            class="w-full h-auto object-cover"
                        />
                    </div>

                    <div class="p-4">
                        <h5 class="text-purple-700 font-semibold text-lg mb-2">
                            {{ course.title }}
                        </h5>
                        <p class="text-gray-600 text-sm leading-relaxed">
                            {{ course.description }}
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
const courses = [
    {
        image: "/images/ct_1.png",
        imageTitle: "Khoá học",
        imageSubtitle: "Kỹ thuật viên Spa chuyên nghiệp",
        title: "Khoá học Spa",
        description:
            "Khoá học Spa đào tạo từ cơ bản đến nâng cao làm đẹp được thiết kế phù hợp với nhu cầu của các học viên nhằm mục đích sau khi kết thúc khoá học có thể làm việc chuyên nghiệp hoặc là mở cơ sở Spa cho riêng mình.",
    },
    {
        image: "/images/ct_2.png",
        imageTitle: "Khoá học",
        imageSubtitle: "Phun xăm thẩm mỹ chuyên nghiệp",
        title: "Khoá học phun xăm",
        description:
            "Khoá học phun xăm đào tạo và rèn luyện kỹ năng nghề phun xăm thẩm mỹ từ cơ bản đến nâng cao. Các kỹ thuật phun xăm thẩm mỹ bao gồm phun môi, phun chân mày, phun mí mắt và các kỹ thuật phun xăm khác.",
    },
    {
        image: "/images/ct_3.png",
        imageTitle: "Khoá học",
        imageSubtitle: "Chăm sóc da chuyên nghiệp",
        title: "Khoá học chăm sóc da",
        description:
            "Khoá học chăm sóc da đào tạo chuyên sâu về các phương pháp và kỹ thuật chăm sóc da để giúp làm đẹp. Khoá học này cung cấp cho học viên kiến thức về chăm sóc da như điều trị mụn, và các phương pháp về da khác.",
    },
];
</script>

<style scoped>
/* Optional: Hover effect */
.card:hover {
    transform: translateY(-2px);
    transition: all 0.3s ease-in-out;
}
</style>
