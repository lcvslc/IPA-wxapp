<template>
    <view class="content">
        <view class="top">
            <text style="">HOME</text>
        </view>
        <view class="top-shadow"></view>
        <view class="title-area">
            <text class="title">International</text>
            <text class="title">Phonetic</text>
            <text class="title">Alphabet</text>
        </view>
        <view class="top-shadow"></view>
        <view class="butten-array">
            <button class="button" hover-class="none" v-on:click="navigate2intro">Introduction</button>
            <button class="button" hover-class="none" v-on:click="navigate2start">Start</button>
            <button class="button" hover-class="none" v-on:click="navigate2about">About</button>
        </view>
    </view>
</template>

<script>
    export default {
        data() {
            return {
            }
        },
        onLoad() {

        },
        methods: {
            navigate2intro: function() {
                uni.navigateTo({
                    url: "../intro/intro"
                })
            },

            navigate2start: function() {
                uni.navigateTo({
                    url: "../start/start"
                })
            },

            navigate2about: function() {
                uni.navigateTo({
                    url: "../about/about"
                })
            }
        }
    }
</script>

<style>
    @import url("/lib/style/text.css");
    @import url("/lib/style/button.css");
</style>
