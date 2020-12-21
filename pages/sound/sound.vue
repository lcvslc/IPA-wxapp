<template>
    <view class="content" style="height: auto;">
        <view class="top">
            <text>SOUND</text>
        </view>
        <view class="top-shadow"></view>
        <view class="title-area-b">
            <text class="title-b">IPA Symbols with Sound</text>
        </view>
        <view class="top-shadow"></view>
        <view class="butten-table">
            <view class="butten-table-category">
                <view class="category-title">Plosive</view>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Bilabial</button>
                <button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('plosive-bilabial-1')">p</button>
                <button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('plosive-bilabial-2')">b</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Alveolar</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">t</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">d</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Retroflex</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">ʈ</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">ɖ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Palatal</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">c</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">ɟ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Velar</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">k</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">g</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Uvular</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">q</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">ɢ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Glottal</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">ʔ</button>
            </view>
            <view class="butten-table-category">
                <view class="category-title">Nasal</view>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Bilabial</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">m</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Labiodental</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">ɱ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Alveolar</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">n</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Retroflex</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">ɳ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Palatal</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">ɲ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Velar</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">ŋ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Uvular</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">ɴ</button>
            </view>
            <view class="butten-table-category">
                <view class="category-title">Trill</view>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Bilabial</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">ʙ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Alveolar</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">r</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Uvular</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">ʀ</button>
            </view>
            <view class="butten-table-category">
                <view class="category-title">Tap or Flap</view>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Labiodental</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">ⱱ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Alveolar</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">ɾ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Retroflex</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">ɽ</button>
            </view>
            <view class="butten-table-category">
                <view class="category-title">Fricative</view>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Bilabial</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">ɸ</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">β</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Labiodental</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">f</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">v</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Dental</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">θ</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">ð</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Alveolar</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">s</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">z</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Postalveolar</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">ʃ</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">ʒ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Retroflex</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">ʂ</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">ʐ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Palatal</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">ç</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">ʝ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Velar</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">x</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">ɣ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Uvular</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">χ</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">ʁ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Pharyngeal</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">ħ</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">ʕ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Glottal</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">h</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">ɦ</button>
            </view>
            <view class="butten-table-category">
                <view class="category-title">Lateral Fricative</view>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Alveolar</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">ɬ</button>
                <button class="button-b" hover-class="none" style="width: 15vw;">ɮ</button>
            </view>
            <view class="butten-table-category">
                <view class="category-title">Approximant</view>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Labiodental</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">ʋ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Alveolar</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">ɹ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Retroflex</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">ɻ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Palatal</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">j</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Velar</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">ɰ</button>
            </view>
            <view class="butten-table-category">
                <view class="category-title">Lateral Approximant</view>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Alveolar</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">l</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Retroflex</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">ɭ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Palatal</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">ʎ</button>
            </view>
            <view class="butten-array-b">
                <button class="button-b" hover-class="none" style="width: 55vw;">Velar</button>
                <button class="button-b" hover-class="none" style="width: 30vw;">ʟ</button>
            </view>
        </view>
        <view class="fill-bottom"></view>
    </view>
</template>

<script>
    export default {
        data() {
            return {
            }
        },
        methods: {
            navigate2more: function (obj) {
                uni.navigateTo({
                    url: "../detail/detail?id=" + obj
                })
            }
        }
    }
</script>

<style>
    @import url("~@/static/text.css");
    @import url("~@/static/button.css");
</style>
