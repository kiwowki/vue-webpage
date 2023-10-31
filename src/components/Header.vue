<template>
  <header id="headerType" :class="['header_wrap', element]">
    <div class="header_inner nexon">
      <div class="header_logo"><a href="/">{{ title }} <em>site</em></a></div>
      <nav class="header_menu">
        <ul>
          <li><a href="/">헤더 영역</a></li>
          <li><a href="/">슬라이드 영역</a></li>
          <li><a href="/">배너 영역</a></li>
          <li><a href="/">컨텐츠 영역</a></li>
          <li><a href="/">푸터 영역</a></li>
        </ul>
      </nav>
      <div class="header_member">
        <a href="/">로그인</a>
      </div>
    </div>
  </header>
</template>
<script>
export default {
  props: {
    element: String,
    title: String,
  }
}
</script>