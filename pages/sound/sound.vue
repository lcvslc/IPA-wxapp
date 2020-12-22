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
                <button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('plosive-alveolar-1')">t</button>
                <button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('plosive-alveolar-2')">d</button>
            </view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Retroflex</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('plosive-retroflex-1')">ʈ</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('plosive-retroflex-2')">ɖ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Palatal</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('plosive-palatal-1')">c</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('plosive-palatal-2')">ɟ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Velar</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('plosive-velar-1')">k</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('plosive-velar-2')">g</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Uvular</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('plosive-uvular-1')">q</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('plosive-uvular-2')">ɢ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Glottal</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('plosive-glottal-1')">ʔ</button>
			</view>
			<view class="butten-table-category">
				<view class="category-title">Nasal</view>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Bilabial</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('nasal-bilabial-1')">m</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Labiodental</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('nasal-labiodental-1')">ɱ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Alveolar</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('nasal-alveolar-1')">n</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Retroflex</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('nasal-retroflex-1')">ɳ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Palatal</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('nasal-palatal1-1')">ɲ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Velar</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('nasal-velar-1')">ŋ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Uvular</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('nasal-uvular-1')">ɴ</button>
			</view>
			<view class="butten-table-category">
				<view class="category-title">Trill</view>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Bilabial</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('trill-bilabial-1')">ʙ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Alveolar</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('trill-alveolar-1')">r</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Uvular</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('trill-uvular-1')">ʀ</button>
			</view>
			<view class="butten-table-category">
				<view class="category-title">Tap or Flap</view>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Alveolar</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('tap-or-flap-alveolar-1')">ɾ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Retroflex</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('tap-or-flap-retroflex-1')">ɽ</button>
			</view>
			<view class="butten-table-category">
				<view class="category-title">Fricative</view>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Bilabial</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-bilabial-1')">ɸ</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-bilabial-2')">β</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Labiodental</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-labiodental-1')">f</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-labiodental-2')">v</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Dental</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-dental-1')">θ</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-dental-2')">ð</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Alveolar</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-alveolar-1')">s</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-alveolar-2')">z</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Postalveolar</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-postalveolar-1')">ʃ</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-postalveolar-2')">ʒ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Retroflex</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-retroflex-1')">ʂ</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-retroflex-2')">ʐ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Palatal</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-palatal-1')">ç</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-palatal-2')">ʝ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Velar</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-velar-1')">x</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-velar-2')">ɣ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Uvular</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-uvular-1')">χ</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-uvular-2')">ʁ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Pharyngeal</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-pharyngeal-1')">ħ</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-pharyngeal-2')">ʕ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Glottal</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-glottal-1')">h</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('fricative-glottal-2')">ɦ</button>
			</view>
			<view class="butten-table-category">
				<view class="category-title">Lateral Fricative</view>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Alveolar</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('lateral-fricative-alveolar-1')">ɬ</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('lateral-fricative-alveolar-2')">ɮ</button>
			</view>
			<view class="butten-table-category">
				<view class="category-title">Approximant</view>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Labiodental</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('approximant-labiodental-1')">ʋ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Alveolar</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('approximant-alveolar-1')">ɹ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Retroflex</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('approximant-retroflex-1')">ɻ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Palatal</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('approximant-palatal-1')">j</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Velar</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('approximant-velar-1')">ɰ</button>
			</view>
			<view class="butten-table-category">
				<view class="category-title">Lateral Approximant</view>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Alveolar</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('lateral-approximant-alveolar-1')">l</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Retroflex</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('lateral-approximant-retroflex-1')">ɭ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Palatal</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('lateral-approximant-palatal-1')">ʎ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Velar</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('lateral-approximant-velar-1')">ʟ</button>
			</view>
			<view class="butten-table-category">
				<view class="category-title">Close</view>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Front</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('close-front-1')">i</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('close-front-2')">y</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Central</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('close-central-1')">ɨ</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('close-central-2')">ʉ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Back</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('close-back-1')">ɯ</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('close-back-2')">u</button>
			</view>
			<view class="butten-table-category">
				<view class="category-title">Near Close</view>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Near Front</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('near-close-near-front-1')">ɪ</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('near-close-near-front-2')">ʏ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Near Back</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('near-close-near-back-1')">ʊ</button>
			</view>
			<view class="butten-table-category">
				<view class="category-title">Close Mid</view>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Front</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('close-mid-front-1')">e</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Near Front</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('close-mid-near-front-1')">ø</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Central</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('close-mid-central-1')">ɘ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Near Back</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('close-mid-near-back-1')">ɵ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Back</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('close-mid-back-1')">ɤ</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('close-mid-back-2')">o</button>
			</view>
			<view class="butten-table-category">
				<view class="category-title">Mid</view>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Central</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('mid-central-1')">ə</button>
			</view>
			<view class="butten-table-category">
				<view class="category-title">Open Mid</view>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Near Front</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('open-mid-near-front-1')">ɛ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Central</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('open-mid-central-1')">œ</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('open-mid-central-2')">ɜ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Near Back</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('open-mid-near-back-1')">ɞ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Back</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('open-mid-back-1')">ʌ</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('open-mid-back-2')">ɔ</button>
			</view>
			<view class="butten-table-category">
				<view class="category-title">Near Open</view>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Near Front</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('near-open-near-front-1')">æ</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Near Back</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('near-open-near-back-1')">ɐ</button>
			</view>
			<view class="butten-table-category">
				<view class="category-title">Open</view>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Central</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('open-central-1')">a</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Near Back</button>
				<button class="button-b" hover-class="none" style="width: 30vw;" v-on:click="navigate2more('open-near-back-1')">ä</button>
			</view>
			<view class="butten-array-b">
				<button class="button-b" hover-class="none" style="width: 55vw;">Back</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('open-back-1')">ɑ</button>
				<button class="button-b" hover-class="none" style="width: 15vw;" v-on:click="navigate2more('open-back-2')">ɒ</button>
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
                    url: "../detail/detail?title=" + obj
                })
            }
        }
    }
</script>

<style>
    @import url("@/static/text.css");
    @import url("@/static/button.css");
</style>
