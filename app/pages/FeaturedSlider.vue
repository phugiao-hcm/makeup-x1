<template>
    <section class="bg-white py-10 px-4">
        <div
            class="max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-2 gap-8 items-center"
        >
            <!-- Video -->
            <div class="aspect-video">
                <iframe
                    class="w-full h-full rounded-xl"
                    src="https://www.youtube.com/embed/cs8-aNRf-h8?si=tQda-_1J-jcf_zy8"
                    title="Video giới thiệu"
                    frameborder="0"
                    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                    referrerpolicy="strict-origin-when-cross-origin"
                    allowfullscreen
                ></iframe>
            </div>

            <!-- Text Content -->
            <div class="space-y-4">
                <span
                    class="inline-block bg-purple-700 text-white font-semibold px-4 py-1 rounded-full text-sm"
                >
                    VỀ CHÚNG TÔI
                </span>

                <h2 class="text-3xl md:text-4xl font-bold text-purple-800">
                    Học viện Thẩm mỹ Royal
                </h2>

                <p class="text-gray-700 leading-relaxed">
                    <span class="text-purple-700 font-medium"
                        >Học viện Thẩm mỹ Royal</span
                    >
                    đơn vị đào tạo <strong>số 1</strong> các khoá học liên quan
                    đến chăm sóc sắc đẹp.
                    <strong>Royal Beauty Academy</strong> cam kết hỗ trợ việc
                    làm cho học viên sau khi tốt nghiệp, đào tạo bài bản với
                    giáo trình bài bản chuyên nghiệp 85% thực hành 15% lý thuyết
                    được biên soạn phù hợp với mỗi khóa học giúp cho học viên
                    học tập tốt hiểu bài nhanh chóng và thực hành ngay tại lớp
                    học đào tạo. Royal Beauty Academy là địa chỉ đào tạo chuyên
                    nghiệp nguồn nhân lực chất lượng cao cho ngành thẩm mỹ, được
                    sự cấp phép của Sở LĐTB&XH TP.HN.
                </p>

                <!-- CTA Buttons -->
                <div class="flex flex-wrap gap-4 pt-2">
                    <a
                        href="#"
                        class="bg-purple-700 text-white px-6 py-2 rounded-full font-semibold shadow hover:bg-purple-800 transition"
                    >
                        TƯ VẤN NGAY <i class="fas fa-arrow-right ml-1"></i>
                    </a>
                    <a
                        href="#"
                        class="border-2 border-purple-700 text-purple-700 px-6 py-2 rounded-full font-semibold hover:bg-purple-50 transition"
                    >
                        XEM CHI TIẾT
                        <i class="fas fa-arrow-circle-right ml-1"></i>
                    </a>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
// No logic needed
</script>

<style scoped>
/* Optional: you can add any custom tweaks */
</style>
