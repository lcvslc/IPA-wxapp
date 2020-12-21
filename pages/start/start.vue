<template>
    <view class="content">
        <view class="top">
            <text>START</text>
        </view>
        <view class="top-shadow"></view>
        <view class="title-area-b">
            <text class="title-b">Content</text>
        </view>
        <view class="top-shadow"></view>
        <view class="butten-array">
            <button class="button" hover-class="none" v-on:click="navigate2chart">Chart</button>
            <button class="button" hover-class="none" v-on:click="navigate2sound">Sound</button>
            <button class="button" hover-class="none" v-on:click="navigate2tones">Tones</button>
            <button class="button" hover-class="none" v-on:click="navigate2vowels">Vowels</button>
            <button class="button" hover-class="none" v-on:click="navigate2pinyin">Pinyin</button>
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
            navigate2chart: function () {
                uni.navigateTo({
                    url: "../chart/chart"
                })
            },
            navigate2sound: function () {
                uni.navigateTo({
                    url: "../sound/sound?id=1&name=test"
                })
            },
            navigate2tones: function () {
                uni.navigateTo({
                    url: "../tones/tones"
                })
            },
            navigate2vowels: function () {
                uni.navigateTo({
                    url: "../vowels/vowels"
                })
            },
            navigate2pinyin: function () {
                uni.navigateTo({
                    url: "../pinyin/pinyin"
                })
            }
        }
    }
</script>

<style>
    @import url("~@/static/text.css");
    @import url("~@/static/button.css");
</style>
