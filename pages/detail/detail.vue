<template>
    <view>
        <view class="top">
            <text>DETAILS</text>
        </view>
    </view>
</template>

<script>
    export default {
        data() {
            return {
                title: "test"
            }
        },
        onLoad: function(obj){
            console.log(obj.id);
            if (obj.id == "plosive-bilabial-1") {
                this.title = "p";
            } else if (obj.id == "plosive-bilabial-2") {
                this.title = "b"
            }
        },
        methods: {
            
        }
    }
</script>

<style>
    @import url("~@/static/text.css");
</style>
