<template>
    <section id="sliderType" :class="['slider_wrap', element]">
        <h2 class="blind">{{ title }}</h2>
        <div class="slider_inner">
            <div class="slider">
                <div class="slider_img">
                    <div class="desc">
                        <span>developer</span>
                        <h3>New Frontend</h3>
                        <p>
                            너무 무리하지 말아요! 이미 당신은 잘 하고 있어요!!<br />
                            앞으로도 잘 할 수 있어요!!!
                        </p>
                        <div class="btn">
                            <a href="/">자세히 보기</a>
                            <a href="/" class="black">사이트 보기</a>
                        </div>
                    </div>
                </div>
                <div class="slider_arrow">
                    <a href="/" class="left"><span class="ir">이전 이미지</span></a>
                    <a href="/" class="right"><span class="ir">다음 이미지</span></a>
                </div>
                <div class="slider_dot">
                    <a href="/" class="dot active"><span class="ir">1</span></a>
                    <a href="/" class="dot"><span class="ir">2</span></a>
                    <a href="/" class="dot"><span class="ir">3</span></a>
                    <a href="/" class="play"><span class="ir">플레이</span></a>
                    <a href="/" class="stop"><span class="ir">정지</span></a>
                </div>
            </div>
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