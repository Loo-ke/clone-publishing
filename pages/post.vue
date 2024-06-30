<template>
  <div>
    <div>비즈니스</div>
    <div>카카오페이의 삼성페이 연동, 과연 잘한걸까요?</div>
    <div>icon username</div>
    <div>
      <div>9분 | 2일 전</div>
      <div>icon 12.1k</div>
    </div>
    <!-- 로그인 유도 -->
    <div>
      <div>
        <div>몇 년차, 어떤 스킬, 어떤 직무의 독자들이 봤을까요?</div>
        <div>
          bg img
          <div>
            <div>어떤 독자들이 봤는지 <br />궁금하다면?</div>
            <button class="border p-2">로그인</button>
          </div>
        </div>
      </div>
    </div>
    <div>
      <div>개 긴 글</div>
      <div>카카오 페이 광고</div>
      <div>
        <div>title</div>
        <div>개 긴 글2-1</div>
        <div>카카오페이 광고 2</div>
        <div>개긴글 2-2</div>
      </div>
      <div>
        원문
        <div>카카오페이의 삼성페이 연동, 잘한 걸까요?</div>
      </div>
    </div>
    <div>
      요즘IT의 모든 콘텐츠는 저작권법의 보호를 받는바, 무단 전재와 복사, 배포
      등을 금합니다.
    </div>
    <div>
      <div>좋아요 , 댓글 수 | 저장, 공유</div>
    </div>
    <div>
      <div>댓글 0</div>
      <div>input 로그인하고 자유롭게 의견을 남겨주세요.</div>
    </div>
    <div class="bg-gray-200">
      <div>user 부분 나오고</div>
      <div>글 리스트3개</div>
      <div>작가의 콘텐츠 더 보기 ></div>
    </div>
    <div>
      <div>같은 분야를 다룬 콘텐츠</div>
      <div>캐러셀</div>
    </div>
    <div>
      <div>인기 있는 콘텐츠</div>
      <div>캐러셀</div>
    </div>
    <contentsSec3
      :title="sec3Data[1].title"
      :btnTitle="sec3Data[1].btnTitle"
      :address="sec3Data[1].address"
      :icon="sec3Data[1].icon"
    />
  </div>
</template>

<script setup>
import { sec3Data } from '~/data/indexData'
</script>
