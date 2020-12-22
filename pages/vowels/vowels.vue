<template>
    <view class="content">
        <view class="top">
            <text>VOWELS</text>
        </view>
        <view class="top-shadow"></view>
        <view class="title-area-b">
            <text class="title-b">Vowels Chart</text>
        </view>
        <view class="top-shadow"></view>
        <image src="/static/images/ipa-vowels.gif" mode="aspectFit" class="image"></image>
        <view class="normal-text-area">
            <text class="normal-text">
                There are two complementary definitions of vowel, one phonetic and the other phonological.
            </text>
            <text class="normal-text">
                In the phonetic definition, a vowel is a sound, such as the English "ah" /ɑː/ or "oh" /oʊ/, produced
                with an open vocal tract; it is median (the air escapes along the middle of the tongue), oral (at least
                some of the airflow must escape through the mouth), frictionless and continuant. There is no
                significant build-up of air pressure at any point above the glottis. This contrasts with consonants,
                such as the English "sh" [ʃ], which have a constriction or closure at some point along the vocal tract.
            </text>
            <text class="normal-text">
                In the phonological definition, a vowel is defined as syllabic, the sound that forms the peak of a
                syllable. A phonetically equivalent but non-syllabic sound is a semivowel. In oral languages,
                phonetic vowels normally form the peak (nucleus) of many or all syllables, whereas consonants form the
                onset and (in languages that have them) coda. Some languages allow other sounds to form the nucleus of
                a syllable, such as the syllabic (i.e., vocalic) l in the English word table [ˈtʰeɪ.bl̩] (when not
                considered to have a weak vowel sound: [ˈtʰeɪ.bəl]) or the syllabic r in the Serbo-Croatian word vrt
                [ʋr̩̂t] "garden".
            </text>
        </view>
    </view>
</template>

<script>
    export default {
        data() {
            return {}
        },
        methods: {

        }
    }
</script>

<style>
    @import url("@/static/text.css");
    @import url("@/static/image.css");
</style>
