<template>
    <div :class="$style.box">
        <div :class="$style.link">
            <router-link :to="'/Bi'">BI </router-link>
            <router-link :to="'/Used'">중고매물보기</router-link>
            <router-link :to="'/Download'">앱 다운로드</router-link>
        </div>
    </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component({
    components: {},
})
export default class LinkView extends Vue {}
</script>

<style lang="scss" module>
@import "@/assets/utils.scss";
.box {
    width: 100%;
}
.link {
    padding-top: 60px;
    padding-bottom: 60px;

    font-size: 24px;

    text-align: center;
    a {
        padding: 40px;
        color: #333333;
        text-decoration-line: none;
        font-size: 18px;
        @include mobile {
            padding: 10px;
        }
    }
}
</style>
