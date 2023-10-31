<template>
    <!-- <section id="textType" :class="['text_wrap', element]">
        <span>{{ title }}</span>
        <h2>스크립트를 익히는 방법</h2>
        <div class="text_inner container">
            <div class="text t1">
                <h3 class="title">검색 이펙트</h3>
                <p class="desc">자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다. 메서드를 통해 쉽게 검색을 만들 수 있습니다</p>
                <a href="/" class="btn">더보기</a>
            </div>
            <div class="text t2">
                <h3 class="title">퀴즈 이펙트</h3>
                <p class="desc">자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다. 메서드를 통해 쉽게 검색을 만들 수 있습니다</p>
                <a href="/" class="btn">더보기</a>
            </div>
            <div class="text t3">
                <h3 class="title">마우스 이펙트</h3>
                <p class="desc">자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다. 메서드를 통해 쉽게 검색을 만들 수 있습니다</p>
                <a href="/" class="btn">더보기</a>
            </div>
            <div class="text t4">
                <h3 class="title">슬라이드 이펙트</h3>
                <p class="desc">자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다. 메서드를 통해 쉽게 검색을 만들 수 있습니다</p>
                <a href="/" class="btn">더보기</a>
            </div>
            <div class="text t5">
                <h3 class="title">패럴랙스 이펙트</h3>
                <p class="desc">자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다. 메서드를 통해 쉽게 검색을 만들 수 있습니다</p>
                <a href="/" class="btn">더보기</a>
            </div>
            <div class="text t6">
                <h3 class="title">게임 이펙트</h3>
                <p class="desc">자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다. 메서드를 통해 쉽게 검색을 만들 수 있습니다</p>
                <a href="/" class="btn">더보기</a>
            </div>
        </div>
    </section> -->
    <section id="textType" class="text_wrap" :class="element">
        <span>{{ title }}</span>
        <h2>스크립트를 익히는 방법</h2>
        <div class="text_inner container">
            <div v-for="(text, index) in textInfo" :key="index" :class="'text t' + (index + 1)">
                <h3 class="text_title">{{ text.title }}</h3>
                <p class="text_desc">{{ text.desc }}</p>
                <a class="text_btn" :href="text.src">더보기</a>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    props: {
        element: String,
        title: String,
    },

    data: function () {
        return {
            textInfo: [
                {
                    title: "검색 이펙트",
                    desc: "자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다. 메서드를 통해 쉽게 검색을 만들 수 있습니다",
                    src: "/"
                },
                {
                    title: "퀴즈 이펙트",
                    desc: "자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다. 메서드를 통해 쉽게 검색을 만들 수 있습니다",
                    src: "/"
                },
                {
                    title: "마우스 이펙트",
                    desc: "자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다. 메서드를 통해 쉽게 검색을 만들 수 있습니다",
                    src: "/"
                },
                {
                    title: "슬라이드 이펙트",
                    desc: "자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다. 메서드를 통해 쉽게 검색을 만들 수 있습니다",
                    src: "/"
                },
                {
                    title: "패럴랙스 이펙트",
                    desc: "자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다. 메서드를 통해 쉽게 검색을 만들 수 있습니다",
                    src: "/"
                },
                {
                    title: "게임 이펙트",
                    desc: "자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다. 메서드를 통해 쉽게 검색을 만들 수 있습니다",
                    src: "/"
                },
            ]
        }
    }
}
</script>