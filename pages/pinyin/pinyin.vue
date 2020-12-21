<template>
    <view class="content">
        <view class="top">
            <text>PINYIN</text>
        </view>
        <view class="top-shadow"></view>
        <view class="title-area-b">
            <text class="title-b">Chinese Pinyin with IPA</text>
        </view>
        <view class="top-shadow"></view>
        <view class="category" style="border: #000000 1rpx solid;">
            <text class="category-title">Initials</text>
        </view>
        <view class="table-text-area">
            <text class="table-text" style="background-color: #8B4513; color: #E4E4E4;">Pinyin</text>
            <text class="table-text" style="background-color: #8B4513; color: #E4E4E4;">IPA</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">b</text>
            <text class="table-text">[p]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">p</text>
            <text class="table-text">[pʰ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">m</text>
            <text class="table-text">[m]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">f</text>
            <text class="table-text">[f]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">d</text>
            <text class="table-text">[t]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">t</text>
            <text class="table-text">[tʰ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">n</text>
            <text class="table-text">[n]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">l</text>
            <text class="table-text">[l]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">g</text>
            <text class="table-text">[k]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">k</text>
            <text class="table-text">[kʰ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">h</text>
            <text class="table-text">[x]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">j</text>
            <text class="table-text">[tɕ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">q</text>
            <text class="table-text">[tɕʰ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ɕ</text>
            <text class="table-text">[ɕ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">z</text>
            <text class="table-text">[ts]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">c</text>
            <text class="table-text">[tsʰ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">s</text>
            <text class="table-text">[s]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">zh</text>
            <text class="table-text">[tʂ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ch</text>
            <text class="table-text">[tʂʰ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">sh</text>
            <text class="table-text">[ʂ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">r</text>
            <text class="table-text">[ʐ]</text>
        </view>
        <view class="category" style="border: #000000 1rpx solid;">
            <text class="category-title">Finals</text>
        </view>
        <view class="table-text-area">
            <text class="table-text" style="background-color: #8B4513; color: #E4E4E4;">Pinyin</text>
            <text class="table-text" style="background-color: #8B4513; color: #E4E4E4;">IPA</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">a</text>
            <text class="table-text">[a]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">o</text>
            <text class="table-text">[o]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">e</text>
            <text class="table-text">[ɤ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">i</text>
            <text class="table-text">[i]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">u</text>
            <text class="table-text">[u]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ü</text>
            <text class="table-text">[y]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ai</text>
            <text class="table-text">[ai]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ü</text>
            <text class="table-text">[y]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ai</text>
            <text class="table-text">[ai]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ei</text>
            <text class="table-text">[ei]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ao</text>
            <text class="table-text">[ɑu]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ou</text>
            <text class="table-text">[ou]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">an</text>
            <text class="table-text">[an]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">en</text>
            <text class="table-text">[ən]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">in</text>
            <text class="table-text">[in]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ang</text>
            <text class="table-text">[ɑŋ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">eng</text>
            <text class="table-text">[əŋ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ong</text>
            <text class="table-text">[uŋ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ing</text>
            <text class="table-text">[iŋ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ia</text>
            <text class="table-text">[ia]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">iao</text>
            <text class="table-text">[iɑu]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ian</text>
            <text class="table-text">[iæn]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">iang</text>
            <text class="table-text">[iɑŋ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ie</text>
            <text class="table-text">[iɛ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">iong</text>
            <text class="table-text">[yŋ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">iou</text>
            <text class="table-text">[iou]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ua</text>
            <text class="table-text">[uɑ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">uo</text>
            <text class="table-text">[uo]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">uai</text>
            <text class="table-text">[uai]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ui</text>
            <text class="table-text">[uei]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">uan</text>
            <text class="table-text">[uan]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">uang</text>
            <text class="table-text">[uɑŋ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">un</text>
            <text class="table-text">[uən]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ueng</text>
            <text class="table-text">[uəŋ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">üe</text>
            <text class="table-text">[yɛ]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">üan</text>
            <text class="table-text">[yæn]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ün</text>
            <text class="table-text">[yn]</text>
        </view>
        <view class="table-text-area">
            <text class="table-text">ng</text>
            <text class="table-text">[ŋ]</text>
        </view>
    </view>
</template>

<script>
    export default {
        data() {
            return {
            }
        },
        methods: {
            
        }
    }
</script>

<style>
    @import url("~@/static/text.css");
</style>
