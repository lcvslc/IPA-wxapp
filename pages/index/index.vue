<template>
    <view class="content">
        <view class="top">
            <text style="">{{title}}</text>
        </view>
        <view class="top-shadow"></view>
        <view class="title-area">
            <text class="title">International</text>
            <text class="title">Phonetic</text>
            <text class="title">Alphabet</text>
        </view>
        <view class="top-shadow"></view>
        <view class="butten-array">
            <button class="button" hover-class="none" v-on:click="navigate2intro">Intro</button>
            <button class="button" hover-class="none" v-on:click="navigate2start">Start</button>
            <button class="button" hover-class="none" v-on:click="navigate2about">About</button>
        </view>
    </view>
</template>

<script>
    export default {
        data() {
            return {
                title: "HOME"
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
    @import url("~@/static/text.css");

    .butten-array {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        background-color: #ffffd7;
        height: 50vh;
    }

    .button {
        margin-top: 5%;
        margin-bottom: 5%;
        width: 50vw;
        border: #000000 5rpx solid;
        box-shadow: 20rpx 10rpx #333333;
    }
</style>
