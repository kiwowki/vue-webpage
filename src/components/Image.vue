<template>
    <section id="imageType" :class="['image_wrap', element]">
        <h2>{{ title }}</h2>
        <p>이미지 유형입니다. 마우스 오버시 자세한 정보가 나오는 구조입니다.</p>
        <div class="image_inner container">
            <article class="image img1">
                <h3 class="image_title">강아지계의 겸둥이</h3>
                <p class="image_desc">무슨 종인지는 모르겠지만 귀여워서 넣어봤습니다. 큰 귀가 매력적입니다. <br />아주 아주 귀엽습니다.</p>
                <!-- <img src="" alt="귀여운 강아지 이미지"> -->
                <a href="/" class="image_btn">자세히 보기</a>
            </article>
            <article class="image img2">
                <h3 class="image_title">강아지계의 사랑둥이</h3>
                <p class="image_desc">새까만 눈이 마지 블랙 올리브 같습니다. 사랑둥이 인정입니다. <br />아주 아주 귀엽습니다.</p>
                <!-- <img src="img/Rectangle9.jpg" alt="귀여운 강아지 이미지"> -->
                <a href="/" class="image_btn yellow">자세히 보기</a>
            </article>
        </div>
    </section>
</template>
<script>
export default {
    props: {
        element: String,
        title: String,
    }
}
</script>