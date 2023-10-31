<script setup>
import Header from "@/components/Header.vue"

import Slider from "@/components/Slider.vue"
import Image from "@/components/Image.vue"
import ImgText from "@/components/ImgText.vue"
import Card from "@/components/Card.vue"
import Banner from "@/components/Banner.vue"
import Text from "@/components/Text.vue"

import Footer from "@/components/Footer.vue"
</script>

<template>
  <Header element="nexon" title="wolves" />
  <main>
    <Slider element="nexon" title="슬라이드 유형" />
    <Image element="nexon section" title="포트폴리오가 실력이다." />
    <ImgText element="section nexon" title="이미지 텍스트 유형" />
    <Card element="nexon container section" title="강서현의 코딩 사이트" />
    <Banner element="" title="배너 영역" />
    <Text element="section" title="텍스트 유형01" />
  </main>
  <Footer element="section" title="푸터 영역" />
</template>
