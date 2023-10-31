<template>
    <section id="cardType" :class="['card_wrap', element]">
        <h2>{{ title }}</h2>
        <p>
            웹디자이너, 웹퍼블리셔, 프론트앤드 개발자가 되기위한 코딩 강의 사이트입니다.<br />
            NEXON Lv1 Gothic OTF 22px 150% #666
        </p>
        <div class="card_inner container">
            <article class="card" v-for="(card, key) in cardInfo" :key="key">
                <figure class="card_header">
                    <img :src="card.img" :alt="card.title" />
                </figure>
                <div class="card_body">
                    <h3 class="title">{{ card.title }}</h3>
                    <p class="desc">{{ card.desc }}</p>
                    <a href="/" class="btn">
                        더 자세히 보기
                        <span aria-hidden="true">
                            <svg width="51" height="8" viewBox="0 0 51 8" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path
                                    d="M50.3536 4.35355C50.5488 4.15829 50.5488 3.84171 50.3536 3.64645L47.1716 0.464466C46.9763 0.269204 46.6597 0.269204 46.4645 0.464466C46.2692 0.659728 46.2692 0.976311 46.4645 1.17157L49.2929 4L46.4645 6.82843C46.2692 7.02369 46.2692 7.34027 46.4645 7.53553C46.6597 7.7308 46.9763 7.7308 47.1716 7.53553L50.3536 4.35355ZM0 4.5H50V3.5H0V4.5Z"
                                    fill="black" />
                            </svg>
                        </span>
                    </a>
                </div>
            </article>
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
            cardInfo: [
                {
                    img: "/src/assets/img/Rectangle17.jpg",
                    title: "웹표준 사이트 만들기",
                    desc: "사이트를 만들기 위한 기초 강의입니다. 기본 코딩에 대한 감각을 익히고, 웹 표준을 준수하면서 코딩하는 방법을 익힙니다. 다양한 예제를 통해 사이트를 만드는 사이트.."
                },
                {
                    img: "/src/assets/img/card01.jpg",
                    title: "반응형 사이트 만들기",
                    desc: "사이트를 만들기 위한 기초 강의입니다. 기본 코딩에 대한 감각을 익히고, 웹 표준을 준수하면서 코딩하는 방법을 익힙니다. 다양한 예제를 통해 사이트를 만드는 사이트.."
                },
                {
                    img: "/src/assets/img/card03.jpg",
                    title: "패럴랙스 사이트 만들기",
                    desc: "사이트를 만들기 위한 기초 강의입니다. 기본 코딩에 대한 감각을 익히고, 웹 표준을 준수하면서 코딩하는 방법을 익힙니다. 다양한 예제를 통해 사이트를 만드는 사이트.."
                }
            ]
        }
    }
}
</script>

<style></style>