<template>
    <view class="content">
        <view class="top">
            <text>{{title}}</text>
        </view>
        <view class="top-shadow"></view>
        <view class="title-area-b">
            <text class="title-b">Vowels Chart</text>
        </view>
        <view class="top-shadow"></view>
        <image src="~@/static/ipa-vowels.gif" mode="aspectFit" class="image"></image>
        <view class="normal-text-area">
            
        </view>
    </view>
</template>

<script>
    export default {
        data() {
            return {
                title: "VOWELS"
            }
        },
        methods: {
            
        }
    }
</script>

<style>
    @import url("~@/static/text.css");
    @import url("~@/static/image.css");
</style>
