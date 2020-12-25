<template>
    <view class="content">
        <view class="top">
            <text>DETAILS</text>
        </view>
        <view class="top-shadow"></view>
        <view class="title-area-b">
            <text class="title-b">IPA Symbols Details</text>
        </view>
        <view class="top-shadow"></view>
        <view class="title-button-area">
            <view class="this-title">[{{title}}]</view>
            <image class="play-button" src="/static/images/audio.svg" mode="aspectFit" v-on:click="playAudio"></image>
        </view>
        <view class="normal-text-area">
            <text class="normal-text">{{feature}}</text>
        </view>
    </view>
</template>

<script>
    export default {
        data() {
            return {
                title: null,
                audioURL: null,
                feature: null
            }
        },
        onLoad: function(obj) {

            if (obj.title == "plosive-bilabial-1") {
                this.title = "p";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiceless_bilabial_plosive.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Since the consonant is also oral, with no nasal outlet, the airflow is blocked entirely, and the consonant is a plosive." +
                    "\n\n" + "Its place of articulation is bilabial, which means it is articulated with both lips." +
                    "\n\n" +
                    "Its phonation is voiceless, which means it is produced without vibrations of the vocal cords. In some languages the vocal cords are actively separated, so it is always voiceless; in others the cords are lax, so that it may take on the voicing of adjacent sounds." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "Because the sound is not produced with airflow over the tongue, the central–lateral dichotomy does not apply." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "plosive-bilabial-2") {
                this.title = "b";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiced_bilabial_plosive.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Since the consonant is also oral, with no nasal outlet, the airflow is blocked entirely, and the consonant is a plosive." +
                    "\n\n" + "Its place of articulation is bilabial, which means it is articulated with both lips." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "Because the sound is not produced with airflow over the tongue, the central–lateral dichotomy does not apply." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "plosive-alveolar-1") {
                this.title = "t";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiceless_alveolar_plosive.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Since the consonant is also oral, with no nasal outlet, the airflow is blocked entirely, and the consonant is a plosive." +
                    "\n\n" + "There are three specific variants of [t]:" +
                    "\n\n" +
                    "    Dental, which means it is articulated with either the tip or the blade of the tongue at the upper teeth, termed respectively apical and laminal." +
                    "\n\n" +
                    "    Denti-alveolar, which means it is articulated with the blade of the tongue at the alveolar ridge, and the tip of the tongue behind upper teeth." +
                    "\n\n" +
                    "    Alveolar, which means it is articulated with either the tip or the blade of the tongue at the alveolar ridge, termed respectively apical and laminal." +
                    "\n\n" +
                    "Its phonation is voiceless, which means it is produced without vibrations of the vocal cords. In some languages the vocal cords are actively separated, so it is always voiceless; in others the cords are lax, so that it may take on the voicing of adjacent sounds." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "plosive-alveolar-2") {
                this.title = "d";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiced_alveolar_plosive.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Since the consonant is also oral, with no nasal outlet, the airflow is blocked entirely, and the consonant is a plosive." +
                    "\n\n" + "There are three specific variants of [d]:"
                "\n\n" +
                "    Dental, which means it is articulated with either the tip or the blade of the tongue at the upper teeth, termed respectively apical and laminal." +
                "\n\n" +
                "    Denti-alveolar, which means it is articulated with the blade of the tongue at the alveolar ridge, and the tip of the tongue behind upper teeth." +
                "\n\n" +
                "    Alveolar, which means it is articulated with either the tip or the blade of the tongue at the alveolar ridge, termed respectively apical and laminal." +
                "\n\n" + "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                "\n\n" + "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                "\n\n" +
                "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                "\n\n" +
                "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "plosive-retroflex-1") {
                this.title = "ʈ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiceless_retroflex_plosive.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Since the consonant is also oral, with no nasal outlet, the airflow is blocked entirely, and the consonant is a plosive." +
                    "\n\n" +
                    "Its place of articulation is retroflex, which prototypically means it is articulated subapical (with the tip of the tongue curled up), but more generally, it means that it is postalveolar without being palatalized. That is, besides the prototypical subapical articulation, the tongue contact can be apical (pointed) or laminal (flat)." +
                    "\n\n" +
                    "Its phonation is voiceless, which means it is produced without vibrations of the vocal cords. In some languages the vocal cords are actively separated, so it is always voiceless; in others the cords are lax, so that it may take on the voicing of adjacent sounds." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "plosive-retroflex-2") {
                this.title = "ɖ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiced_retroflex_plosive.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Since the consonant is also oral, with no nasal outlet, the airflow is blocked entirely, and the consonant is a plosive." +
                    "\n\n" +
                    "Its place of articulation is retroflex, which prototypically means it is articulated subapical (with the tip of the tongue curled up), but more generally, it means that it is postalveolar without being palatalized. That is, besides the prototypical subapical articulation, the tongue contact can be apical (pointed) or laminal (flat)."
                "\n\n" + "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                "\n\n" + "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                "\n\n" +
                "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                "\n\n" +
                "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "plosive-palatal-1") {
                this.title = "c";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiceless_palatal_plosive.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Since the consonant is also oral, with no nasal outlet, the airflow is blocked entirely, and the consonant is a plosive." +
                    "\n\n" +
                    "Its place of articulation is palatal, which means it is articulated with the middle or back part of the tongue raised to the hard palate. The otherwise identical post-palatal variant is articulated slightly behind the hard palate, making it sound slightly closer to the velar [k]." +
                    "\n\n" +
                    "Its phonation is voiceless, which means it is produced without vibrations of the vocal cords. Insome languages the vocal cords are actively separated, so it is always voiceless; in others the cords are lax, so that it may take on the voicing of adjacent sounds." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "plosive-palatal-2") {
                this.title = "ɟ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiced_palatal_plosive.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Since the consonant is also oral, with no nasal outlet, the airflow is blocked entirely, and the consonant is a plosive." +
                    "\n\n" +
                    "Its place of articulation is palatal, which means it is articulated with the middle or back part of the tongue raised to the hard palate. The otherwise identical post-palatal variant is articulated slightly behind the hard palate, making it sound slightly closer to the velar [ɡ]." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "plosive-velar-1") {
                this.title = "k";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiceless_velar_plosive.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Since the consonant is also oral, with no nasal outlet, the airflow is blocked entirely, and the consonant is a plosive." +
                    "\n\n" +
                    "Its place of articulation is velar, which means it is articulated with the back of the tongue (the dorsum) at the soft palate." +
                    "\n\n" +
                    "Its phonation is voiceless, which means it is produced without vibrations of the vocal cords. Insome languages the vocal cords are actively separated, so it is always voiceless; in others the cords are lax, so that it may take on the voicing of adjacent sounds." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "plosive-velar-2") {
                this.title = "g";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiced_velar_plosive.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Since the consonant is also oral, with no nasal outlet, the airflow is blocked entirely, and the consonant is a plosive." +
                    "\n\n" +
                    "Its place of articulation is velar, which means it is articulated with the back of the tongue (the dorsum) at the soft palate." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "plosive-uvular-1") {
                this.title = "q";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiceless_uvular_plosive.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Since the consonant is also oral, with no nasal outlet, the airflow is blocked entirely, and the consonant is a plosive." +
                    "\n\n" +
                    "Its place of articulation is uvular, which means it is articulated with the back of the tongue (the dorsum) at the uvula." +
                    "\n\n" +
                    "Its phonation is voiceless, which means it is produced without vibrations of the vocal cords. Insome languages the vocal cords are actively separated, so it is always voiceless; in others the cords are lax, so that it may take on the voicing of adjacent sounds." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "plosive-uvular-2") {
                this.title = "ɢ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiced_uvular_plosive.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Since the consonant is also oral, with no nasal outlet, the airflow is blocked entirely, and the consonant is a plosive." +
                    "\n\n" +
                    "Its place of articulation is uvular, which means it is articulated with the back of the tongue (the dorsum) at the uvula." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "plosive-glottal-1") {
                this.title = "ʔ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Glottal_stop.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Since the consonant is also oral, with no nasal outlet, the airflow is blocked entirely, and the consonant is a plosive." +
                    "\n\n" +
                    "Its place of articulation is glottal, which means it is articulated at and by the vocal cords (vocal folds)."
                "\n\n" +
                "It has no phonation, as there is no airflow through the glottis. It is voiceless, however, in the sense that it is produced without vibration of the vocal cords." +
                "\n\n" + "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                "\n\n" +
                "Because the soundis not produced with airflow over the tongue, the central–lateral dichotomy does not apply." +
                "\n\n" +
                "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "nasal-bilabial-1") {
                this.title = "m";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Bilabial_nasal.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Because the consonant is also nasal, the blocked airflow is redirected through the nose." +
                    "\n\n" + "Its place of articulation is bilabial, which means it is articulated with both lips." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is a nasal consonant, which means air is allowed to escape through the nose, either exclusively (nasal stops) or in addition to through the mouth." +
                    "\n\n" +
                    "Because the soundis not produced with airflow over the tongue, the central–lateral dichotomy does not apply." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "nasal-labiodental-1") {
                this.title = "ɱ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Labiodental_nasal.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Because the consonant is also nasal, the blocked airflow is redirected through the nose." +
                    "\n\n" +
                    "Its place of articulation is labiodental, which means it is articulated with the lower lip and the upper teeth." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is a nasal consonant, which means air is allowed to escape through the nose, either exclusively (nasal stops) or in addition to through the mouth." +
                    "\n\n" +
                    "Because the soundis not produced with airflow over the tongue, the central–lateral dichotomy does not apply." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "nasal-alveolar-1") {
                this.title = "n";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3//Alveolar_nasal.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Because the consonant is also nasal, the blocked airflow is redirected through the nose." +
                    "\n\n" + "There are four specific variants of [n]:" +
                    "\n\n" +
                    "    Dental, which means it is articulated with either the tip or the blade of the tongue at the upper teeth, termed respectively apical and laminal." +
                    "\n\n" +
                    "    Denti-alveolar, which means it is articulated with the blade of the tongue at the alveolar ridge, and the tip of the tongue behind upper teeth." +
                    "\n\n" +
                    "    Alveolar, which means it is articulated with either the tip or the blade of the tongue at the alveolar ridge, termed respectively apical and laminal." +
                    "\n\n" +
                    "    Postalveolar, which means it is articulated with either the tip or the blade of the tongue behind the alveolar ridge, termed respectively apical and laminal." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is a nasal consonant, which means air is allowed to escape through the nose, either exclusively (nasal stops) or in addition to through the mouth." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "nasal-retroflex-1") {
                this.title = "ɳ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Retroflex_nasal.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Because the consonant is also nasal, the blocked airflow is redirected through the nose." +
                    "\n\n" +
                    "Its place of articulation is retroflex, which prototypically means it is articulated subapical (with the tip of the tongue curled up), but more generally, it means that it is postalveolar without being palatalized. That is, besides the prototypical subapical articulation, the tongue contact can be apical (pointed) or laminal (flat)."
                "\n\n" + "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                "\n\n" +
                "It is a nasal consonant, which means air is allowed to escape through the nose, either exclusively (nasal stops) or in addition to through the mouth." +
                "\n\n" +
                "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                "\n\n" +
                "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "nasal-palatal1-1") {
                this.title = "ɲ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Palatal_nasal.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Because the consonant is also nasal, the blocked airflow is redirected through the nose." +
                    "\n\n" +
                    "Its place of articulation is palatal, which means it is articulated with the middle or back part of the tongue raised to the hard palate." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is a nasal consonant, which means air is allowed to escape through the nose, either exclusively (nasal stops) or in addition to through the mouth." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "nasal-velar-1") {
                this.title = "ŋ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Velar_nasal.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Because the consonant is also nasal, the blocked airflow is redirected through the nose." +
                    "\n\n" +
                    "Its place of articulation is velar, which means it is articulated with the back of the tongue (the dorsum) at the soft palate." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is a nasal consonant, which means air is allowed to escape through the nose, either exclusively (nasal stops) or in addition to through the mouth." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "nasal-uvular-1") {
                this.title = "ɴ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Uvular_nasal.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is occlusive, which means it is produced by obstructing airflow in the vocal tract. Because the consonant is also nasal, the blocked airflow is redirected through the nose." +
                    "\n\n" +
                    "Its place of articulation is uvular, which means it is articulated with the back of the tongue (the dorsum) at the uvula." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is a nasal consonant, which means air is allowed to escape through the nose, either exclusively (nasal stops) or in addition to through the mouth." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "trill-bilabial-1") {
                this.title = "ʙ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Bilabial_trill.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is trill, which means it is produced by directing air over an articulator so that it vibrates. Inmost instances, it is only found as the trilled release of a prenasalized stop." +
                    "\n\n" + "Its place of articulation is bilabial, which means it is articulated with both lips." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "Because the soundis not produced with airflow over the tongue, the central–lateral dichotomy does not apply." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "trill-alveolar-1") {
                this.title = "r";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Alveolar_trill.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is trill, which means it is produced by directing air over an articulator so that it vibrates." +
                    "\n\n" + "Its place of articulation may be." +
                    "\n\n" + "    Dental (behind the upper front teeth)." +
                    "\n\n" + "    Alveolar (at the alveolar ridge), or." +
                    "\n\n" + "    post-alveolar (behind the alveolar ridge)." +
                    "\n\n" + "It is most often apical, which means it is pronounced with the tip of the tongue." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "trill-uvular-1") {
                this.title = "ʀ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Uvular_trill.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is trill, which means it is produced by directing air over an articulator so that it vibrates. Unlike in tongue-tip trills, it is the uvula, not the tongue, that vibrates." +
                    "\n\n" +
                    "Its place of articulation is uvular, which means it is articulated with the back of the tongue (the dorsum) at the uvula." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "tap-or-flap-alveolar-1") {
                this.title = "ɾ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Alveolar_tap.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is tap or flap, which means it is produced with a single contraction of the muscles so that the tongue makes very brief contact." +
                    "\n\n" +
                    "Its place of articulation is dental or alveolar, which means it is articulated behind upper front teeth or at the alveolar ridge. It is most often apical, which means that it is pronounced with the tip of the tongue." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "tap-or-flap-retroflex-1") {
                this.title = "ɽ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Retroflex_flap.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is tap or flap, which means it is produced with a single contraction of the muscles so that one articulator (usually the tongue) is thrown against another." +
                    "\n\n" +
                    "Its place of articulation is retroflex, which prototypically means it is articulated subapical (with the tip of the tongue curled up), but more generally, it means that it is postalveolar without being palatalized. That is, besides the prototypical subapical articulation, the tongue contact can be apical (pointed) or laminal (flat)."
                "\n\n" + "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                "\n\n" + "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                "\n\n" +
                "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                "\n\n" +
                "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-bilabial-1") {
                this.title = "ɸ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiceless_bilabial_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is fricative, which means it is produced by constricting air flow through a narrow channel at the place of articulation, causing turbulence." +
                    "\n\n" + "Its place of articulation is bilabial, which means it is articulated with both lips." +
                    "\n\n" +
                    "Its phonation is voiceless, which means it is produced without vibrations of the vocal cords. Insome languages the vocal cords are actively separated, so it is always voiceless; in others the cords are lax, so that it may take on the voicing of adjacent sounds." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "Because the soundis not produced with airflow over the tongue, the central–lateral dichotomy does not apply." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-bilabial-2") {
                this.title = "β";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiced_bilabial_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is fricative, which means it is produced by constricting air flow through a narrow channel at the place of articulation, causing turbulence." +
                    "\n\n" + "Its place of articulation is bilabial, which means it is articulated with both lips." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "Because the soundis not produced with airflow over the tongue, the central–lateral dichotomy does not apply." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-labiodental-1") {
                this.title = "f";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiceless_labiodental_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is fricative, which means it is produced by constricting air flow through a narrow channel at the place of articulation, causing turbulence." +
                    "\n\n" +
                    "Its place of articulation is labiodental, which means it is articulated with the lower lip and the upper teeth." +
                    "\n\n" +
                    "Its phonation is voiceless, which means it is produced without vibrations of the vocal cords. Insome languages the vocal cords are actively separated, so it is always voiceless; in others the cords are lax, so that it may take on the voicing of adjacent sounds." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "Because the soundis not produced with airflow over the tongue, the central–lateral dichotomy does not apply." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-labiodental-2") {
                this.title = "v";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiced_labiodental_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is fricative, which means it is produced by constricting air flow through a narrow channel at the place of articulation, causing turbulence." +
                    "\n\n" +
                    "Its place of articulation is labiodental, which means it is articulated with the lower lip and the upper teeth." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "Because the soundis not produced with airflow over the tongue, the central–lateral dichotomy does not apply." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-dental-1") {
                this.title = "θ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiceless_dental_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is fricative, which means it is produced by constricting air flow through a narrow channel at the place of articulation, causing turbulence. It does not have the grooved tongue and directed airflow, or the high frequencies, of a sibilant." +
                    "\n\n" +
                    "Its place of articulation is dental, which means it is articulated with either the tip or the blade of the tongue at the upper teeth, termed respectively apical and laminal. Note that most stops and liquids described as dental are actually denti-alveolar." +
                    "\n\n" +
                    "Its phonation is voiceless, which means it is produced without vibrations of the vocal cords. Insome languages the vocal cords are actively separated, so it is always voiceless; in others the cords are lax, so that it may take on the voicing of adjacent sounds." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-dental-2") {
                this.title = "ð";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiced_dental_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is fricative, which means it is produced by constricting air flow through a narrow channel at the place of articulation, causing turbulence. It does not have the grooved tongue and directed airflow, or the high frequencies, of a sibilant." +
                    "\n\n" +
                    "Its place of articulation is dental, which means it is articulated with either the tip or the blade of the tongue at the upper teeth, termed respectively apical and laminal. Note that most stops and liquids described as dental are actually denti-alveolar." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-alveolar-1") {
                this.title = "s";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiceless_alveolar_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is sibilant fricative, which means it is generally produced by channeling air flow along a groove in the back of the tongue up to the place of articulation, at which point it is focused against the sharp edge of the nearly clenched teeth, causing high-frequency turbulence." +
                    "\n\n" + "There are at least three specific variants of [s]:" +
                    "\n\n" +
                    "    Dentalized laminal alveolar (commonly called \"dental\"), which means it is articulated with the tongue blade very close to the upper front teeth, with the tongue tip resting behind lower front teeth. The hissing effect in this variety of [s] is very strong."
                "\n\n" +
                "    Non-retracted alveolar, which means it is articulated with either the tip or the blade of the tongue at the alveolar ridge, termed respectively apical and laminal. According to Ladefoged & Maddieson (1996) about half of English speakers use a non-retracted apical articulation." +
                "\n\n" +
                "    Retracted alveolar, which means it is articulated with either the tip or the blade of the tongue slightly behind the alveolar ridge, termed respectively apical and laminal. Acoustically, it is close to laminal [ʂ] or (to a lesser extent) [ʃ]." +
                "\n\n" +
                "Its phonation is voiceless, which means it is produced without vibrations of the vocal cords. Insome languages the vocal cords are actively separated, so it is always voiceless; in others the cords are lax, so that it may take on the voicing of adjacent sounds." +
                "\n\n" + "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                "\n\n" +
                "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                "\n\n" +
                "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-alveolar-2") {
                this.title = "z";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiced_alveolar_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is sibilant fricative, which means it is generally produced by channeling air flow along a groove in the back of the tongue up to the place of articulation, at which point it is focused against the sharp edge of the nearly clenched teeth, causing high-frequency turbulence." +
                    "\n\n" + "There are at least three specific variants of [z]:" +
                    "\n\n" +
                    "    Dentalized laminal alveolar (commonly called \"dental\"), which means it is articulated with the tongue blade very close to the upper front teeth, with the tongue tip resting behind lower front teeth. The hissing effect in this variety of [z] is very strong."
                "\n\n" +
                "    Non-retracted alveolar, which means it is articulated with either the tip or the blade of the tongue at the alveolar ridge, termed respectively apical and laminal. According to Ladefoged & Maddieson (1996) about half of English speakers use a non-retracted apical articulation." +
                "\n\n" +
                "    Retracted alveolar, which means it is articulated with either the tip or the blade of the tongue slightly behind the alveolar ridge, termed respectively apical and laminal. Acoustically, it is close to [ʒ] or laminal [ʐ]." +
                "\n\n" + "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                "\n\n" + "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                "\n\n" +
                "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                "\n\n" +
                "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-postalveolar-1") {
                this.title = "ʃ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiceless_postalveolar_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is sibilant fricative, which means it is generally produced by channeling air flow along a groove in the back of the tongue up to the place of articulation, at which point it is focused against the sharp edge of the nearly clenched teeth, causing high-frequency turbulence." +
                    "\n\n" +
                    "Its place of articulation is palato-alveolar, that is, domed (partially palatalized) postalveolar, which means it is articulated with the blade of the tongue behind the alveolar ridge, and the front of the tongue bunched up (\"domed\") at the palate." +
                    "\n\n" +
                    "Its phonation is voiceless, which means it is produced without vibrations of the vocal cords. Insome languages the vocal cords are actively separated, so it is always voiceless; in others the cords are lax, so that it may take on the voicing of adjacent sounds." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-postalveolar-2") {
                this.title = "ʒ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiced_postalveolar_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is sibilant fricative, which means it is generally produced by channeling air flow along a groove in the back of the tongue up to the place of articulation, at which point it is focused against the sharp edge of the nearly clenched teeth, causing high-frequency turbulence." +
                    "\n\n" +
                    "Its place of articulation is palato-alveolar, that is, domed (partially palatalized) postalveolar, which means it is articulated with the blade of the tongue behind the alveolar ridge, and the front of the tongue bunched up (\"domed\") at the palate." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-retroflex-1") {
                this.title = "ʂ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiceless_retroflex_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is sibilant fricative, which means it is generally produced by channeling air flow along a groove in the back of the tongue up to the place of articulation, at which point it is focused against the sharp edge of the nearly clenched teeth, causing high-frequency turbulence." +
                    "\n\n" +
                    "Its place of articulation is retroflex, which prototypically means it is articulated subapical (with the tip of the tongue curled up), but more generally, it means that it is postalveolar without being palatalized. That is, besides the prototypical subapical articulation, the tongue contact can be apical (pointed) or laminal (flat)."
                "\n\n" +
                "Its phonation is voiceless, which means it is produced without vibrations of the vocal cords. Insome languages the vocal cords are actively separated, so it is always voiceless; in others the cords are lax, so that it may take on the voicing of adjacent sounds." +
                "\n\n" + "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                "\n\n" +
                "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                "\n\n" +
                "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-retroflex-2") {
                this.title = "ʐ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiced_retroflex_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is sibilant fricative, which means it is generally produced by channeling air flow along a groove in the back of the tongue up to the place of articulation, at which point it is focused against the sharp edge of the nearly clenched teeth, causing high-frequency turbulence." +
                    "\n\n" +
                    "Its place of articulation is retroflex, which prototypically means it is articulated subapical (with the tip of the tongue curled up), but more generally, it means that it is postalveolar without being palatalized. That is, besides the prototypical subapical articulation, the tongue contact can be apical (pointed) or laminal (flat)."
                "\n\n" + "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                "\n\n" + "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                "\n\n" +
                "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                "\n\n" +
                "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-palatal-1") {
                this.title = "ç";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiceless_palatal_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is fricative, which means it is produced by constricting air flow through a narrow channel at the place of articulation, causing turbulence." +
                    "\n\n" +
                    "Its place of articulation is palatal, which means it is articulated with the middle or back part of the tongue raised to the hard palate. The otherwise identical post-palatal variant is articulated slightly behind the hard palate, making it sound slightly closer to the velar [x]." +
                    "\n\n" +
                    "Its phonation is voiceless, which means it is produced without vibrations of the vocal cords. Insome languages the vocal cords are actively separated, so it is always voiceless; in others the cords are lax, so that it may take on the voicing of adjacent sounds." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-palatal-2") {
                this.title = "ʝ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiced_palatal_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is fricative, which means it is produced by constricting air flow through a narrow channel at the place of articulation, causing turbulence." +
                    "\n\n" +
                    "Its place of articulation is palatal, which means it is articulated with the middle or back part of the tongue raised to the hard palate. The otherwise identical post-palatal variant is articulated slightly behind the hard palate, making it sound slightly closer to the velar [ɣ]." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-velar-1") {
                this.title = "x";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiceless_velar_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is fricative, which means it is produced by constricting air flow through a narrow channel at the place of articulation, causing turbulence." +
                    "\n\n" +
                    "Its place of articulation is velar, which means it is articulated with the back of the tongue (the dorsum) at the soft palate." +
                    "\n\n" +
                    "Its phonation is voiceless, which means it is produced without vibrations of the vocal cords. Insome languages the vocal cords are actively separated, so it is always voiceless; in others the cords are lax, so that it may take on the voicing of adjacent sounds." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-velar-2") {
                this.title = "ɣ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiced_velar_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is fricative, which means it is produced by constricting air flow through a narrow channel at the place of articulation, causing turbulence." +
                    "\n\n" +
                    "Its place of articulation is velar, which means it is articulated with the back of the tongue (the dorsum) at the soft palate." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-uvular-1") {
                this.title = "χ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiceless_uvular_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is fricative, which means it is produced by constricting air flow through a narrow channel at the place of articulation, causing turbulence." +
                    "\n\n" +
                    "Its place of articulation is uvular, which means it is articulated with the back of the tongue (the dorsum) at the uvula." +
                    "\n\n" +
                    "Its phonation is voiceless, which means it is produced without vibrations of the vocal cords. Insome languages the vocal cords are actively separated, so it is always voiceless; in others the cords are lax, so that it may take on the voicing of adjacent sounds." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-uvular-2") {
                this.title = "ʁ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiced_uvular_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is fricative, which means it is produced by constricting air flow through a narrow channel at the place of articulation, causing turbulence. Inmany languages it is closer to an approximant, however, and no language distinguishes the two at the uvular articulation." +
                    "\n\n" +
                    "Its place of articulation is uvular, which means it is articulated with the back of the tongue (the dorsum) at the uvula." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-pharyngeal-1") {
                this.title = "ħ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiceless_pharyngeal_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is fricative, which means it is produced by constricting air flow through a narrow channel at the place of articulation, causing turbulence." +
                    "\n\n" +
                    "Its place of articulation is pharyngeal, which means it is articulated with the tongue root against the back of the throat (the pharynx)."
                "\n\n" +
                "Its phonation is voiceless, which means it is produced without vibrations of the vocal cords. Insome languages the vocal cords are actively separated, so it is always voiceless; in others the cords are lax, so that it may take on the voicing of adjacent sounds." +
                "\n\n" + "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                "\n\n" +
                "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                "\n\n" +
                "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-pharyngeal-2") {
                this.title = "ʕ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiced_pharyngeal_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation varies between approximant and fricative, which means it is produced by narrowing the vocal tract at the place of articulation, but generally not enough to produce much turbulence in the airstream. Languages do not distinguish voiced fricatives from approximants produced in the throat." +
                    "\n\n" +
                    "Its place of articulation is pharyngeal, which means it is articulated with the tongue root against the back of the throat (the pharynx)."
                "\n\n" + "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                "\n\n" + "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                "\n\n" +
                "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                "\n\n" +
                "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-glottal-1") {
                this.title = "h";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiceless_glottal_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "In some languages, it has the constricted manner of articulation of a fricative. However, in many if not most, It is a transitional state of the glottis, with no manner of articulation other than Its phonation type. Because there is no other constriction to produce friction in the vocal tract in the languages they are familiar with, many phoneticians[who?] no longer consider [h] to be a fricative. However, the term \"fricative\" is generally retained for historical reasons." +
                    "\n\n" +
                    "It may have a glottal place of articulation. However, it may have no fricative articulation, in which case the term 'glottal' only refers to the nature of Its phonation, and does not describe the location of the stricture nor the turbulence. All consonants except for the glottals, and all vowels, have an individual place of articulation in addition to the state of the glottis. with all other consonants, surrounding vowels influence the pronunciation [h], and [h] has sometimes been presented as a voiceless vowel, having the place of articulation of these surrounding vowels." +
                    "\n\n" +
                    "Its phonation is voiceless, which means it is produced without vibrations of the vocal cords. Insome languages the vocal cords are actively separated, so it is always voiceless; in others the cords are lax, so that it may take on the voicing of adjacent sounds." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "Because the soundis not produced with airflow over the tongue, the central–lateral dichotomy does not apply." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "fricative-glottal-2") {
                this.title = "ɦ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiced_glottal_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its phonation is breathy voiced, or murmured, which means the vocal cords are loosely vibrating, with more air escaping than in a modally voiced sound. It is sometimes referred to as a \"voiced h\". Strictly speaking this is incorrect, as there is no voicing." +
                    "\n\n" +
                    "In some languages, it has the constricted manner of articulation of a fricative. However, in many if not most, It is a transitional state of the glottis with no manner of articulation other than its phonation type. Because there is no other constriction to produce friction in the vocal tract, most phoneticians no longer consider [ɦ] to be a fricative. True fricatives may have a murmured phonation in addition to producing friction elsewhere. However, the term \"fricative\" is generally retained for the historical reasons." +
                    "\n\n" +
                    "It may have a glottal place of articulation. However, it may have no fricative articulation, making the term glottal mean that it is articulated by the vocal folds, but this is the nature of its phonation rather than a separate articulation. All consonants except for the glottals, and all vowels, have an individual place of articulation in addition to the state of the glottis. As with all other consonants, surrounding vowels influence the pronunciation [ɦ], and accordingly [ɦ] has only the place of articulation of these surrounding vowels." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "Because the soundis not produced with airflow over the tongue, the central–lateral dichotomy does not apply." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "lateral-fricative-alveolar-1") {
                this.title = "ɬ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiceless_alveolar_lateral_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is fricative, which means it is produced by constricting air flow through a narrow channel at the place of articulation, causing turbulence." +
                    "\n\n" +
                    "Its place of articulation is alveolar, which means it is articulated with either the tip or the blade of the tongue at the alveolar ridge, termed respectively apical and laminal." +
                    "\n\n" +
                    "Its phonation is voiceless, which means it is produced without vibrations of the vocal cords. Insome languages the vocal cords are actively separated, so it is always voiceless; in others the cords are lax, so that it may take on the voicing of adjacent sounds." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a lateral consonant, which means it is produced by directing the airstream over the sides of the tongue, rather than down the middle." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "lateral-fricative-alveolar-2") {
                this.title = "ɮ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiceless_alveolar_lateral_fricative.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is fricative, which means it is produced by constricting air flow through a narrow channel at the place of articulation, causing turbulence." +
                    "\n\n" +
                    "Its place of articulation is alveolar, which means it is articulated with either the tip or the blade of the tongue at the alveolar ridge, termed respectively apical and laminal." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a lateral consonant, which means it is produced by directing the airstream over the sides of the tongue, rather than down the middle." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "approximant-labiodental-1") {
                this.title = "ʋ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Labiodental_approximant.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is approximant, which means it is produced by narrowing the vocal tract at the place of articulation, but not enough to produce a turbulent airstream." +
                    "\n\n" +
                    "Its place of articulation is labiodental, which means it is articulated with the lower lip and the upper teeth." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "Because the soundis not produced with airflow over the tongue, the central–lateral dichotomy does not apply." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "approximant-alveolar-1") {
                this.title = "ɹ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Alveolar_approximant.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is approximant, which means it is produced by narrowing the vocal tract at the place of articulation, but not enough to produce a turbulent airstream." +
                    "\n\n" +
                    "Its place of articulation is alveolar, which means it is articulated with either the tip or the blade of the tongue at the alveolar ridge, termed respectively apical and laminal." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "approximant-retroflex-1") {
                this.title = "ɻ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Retroflex_approximant.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is approximant, which means it is produced by narrowing the vocal tract at the place of articulation, but not enough to produce a turbulent airstream." +
                    "\n\n" +
                    "Its place of articulation is retroflex, which prototypically means it is articulated subapical (with the tip of the tongue curled up), but more generally, it means that it is postalveolar without being palatalized. That is, besides the prototypical subapical articulation, the tongue contact can be apical (pointed) or laminal (flat)."
                "\n\n" + "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                "\n\n" + "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                "\n\n" +
                "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                "\n\n" +
                "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "approximant-palatal-1") {
                this.title = "j";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Palatal_approximant.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is approximant, which means it is produced by narrowing the vocal tract at the place of articulation, but not enough to produce a turbulent airstream. The most common type of this approximant is glide or semivowel. The term glide emphasizes the characteristic of movement (or 'glide') of [j] from the [i] vowel position to a following vowel position. The term semivowel emphasizes that, although the sound is vocalic in nature, it is not 'syllabic' (it does not form the nucleus of a syllable).  For a description of the approximant consonant variant used e.g. InSpanish, see above." +
                    "\n\n" +
                    "Its place of articulation is palatal, which means it is articulated with the middle or back part of the tongue raised to the hard palate. The otherwise identical post-palatal variant is articulated slightly behind the hard palate, making it sound slightly closer to the velar [ɰ]." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "approximant-velar-1") {
                this.title = "ɰ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Voiced_velar_approximant.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is approximant, which means it is produced by narrowing the vocal tract at the place of articulation, but not enough to produce a turbulent airstream. The most common type of this approximant is glide or semivowel. The term glide emphasizes the characteristic of movement (or 'glide') of [ɰ] from the [ɯ] vowel position to a following vowel position. The term semivowel emphasizes that, although the sound is vocalic in nature, it is not 'syllabic' (it does not form the nucleus of a syllable).  For a description of the approximant consonant variant used e.g. InSpanish, see below." +
                    "\n\n" +
                    "Its place of articulation is velar, which means it is articulated with the back of the tongue (the dorsum) at the soft palate." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a central consonant, which means it is produced by directing the airstream along the center of the tongue, rather than to the sides." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "lateral-approximant-alveolar-1") {
                this.title = "l";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Alveolar_lateral_approximant.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is approximant, which means it is produced by narrowing the vocal tract at the place of articulation, but not enough to produce a turbulent airstream." +
                    "\n\n" + "There are four specific variants of [l]:" +
                    "\n\n" +
                    "    Dental, which means it is articulated with either the tip or the blade of the tongue at the upper teeth, termed respectively apical and laminal." +
                    "\n\n" +
                    "    Denti-alveolar, which means it is articulated with the blade of the tongue at the alveolar ridge, and the tip of the tongue behind upper teeth." +
                    "\n\n" +
                    "    Alveolar, which means it is articulated with either the tip or the blade of the tongue at the alveolar ridge, termed respectively apical and laminal." +
                    "\n\n" +
                    "    Postalveolar, which means it is articulated with either the tip or the blade of the tongue behind the alveolar ridge, termed respectively apical and laminal." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a lateral consonant, which means it is produced by directing the airstream over the sides of the tongue, rather than down the middle." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "lateral-approximant-retroflex-1") {
                this.title = "ɭ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Retroflex_lateral_approximant.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is approximant, which means it is produced by narrowing the vocal tract at the place of articulation, but not enough to produce a turbulent airstream." +
                    "\n\n" +
                    "Its place of articulation is retroflex, which prototypically means it is articulated subapical (with the tip of the tongue curled up), but more generally, it means that it is postalveolar without being palatalized. That is, besides the prototypical subapical articulation, the tongue contact can be apical (pointed) or laminal (flat)."
                "\n\n" + "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                "\n\n" + "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                "\n\n" +
                "It is a lateral consonant, which means it is produced by directing the airstream over the sides of the tongue, rather than down the middle." +
                "\n\n" +
                "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "lateral-approximant-palatal-1") {
                this.title = "ʎ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Palatal_lateral_approximant.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is approximant, which means it is produced by narrowing the vocal tract at the place of articulation, but not enough to produce a turbulent airstream." +
                    "\n\n" +
                    "Its place of articulation is palatal, which means it is articulated with the middle or back part of the tongue raised to the hard palate." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a lateral consonant, which means it is produced by directing the airstream over the sides of the tongue, rather than down the middle." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "lateral-approximant-velar-1") {
                this.title = "ʟ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Velar_lateral_approximant.mp3";
                this.feature =
                    "\n\n" +
                    "Its manner of articulation is approximant, which means it is produced by narrowing the vocal tract at the place of articulation, but not enough to produce a turbulent airstream." +
                    "\n\n" +
                    "Its place of articulation is velar, which means it is articulated with the back of the tongue (the dorsum) at the soft palate." +
                    "\n\n" +
                    "Its phonation is voiced, which means the vocal cords vibrate during the articulation." +
                    "\n\n" +
                    "It is an oral consonant, which means air is allowed to escape through the mouth only." +
                    "\n\n" +
                    "It is a lateral consonant, which means it is produced by directing the airstream over the sides of the tongue, rather than down the middle." +
                    "\n\n" +
                    "The airstream mechanism is pulmonic, which means it is articulated by pushing air solely with the lungs and diaphragm, as in most sounds."
            } else if (obj.title == "close-front-1") {
                this.title = "i";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Close_front_unrounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is close, also known as high, which means the tongue is positioned close to the roof of the mouth without creating a constriction that would be classified as a consonant." +
                    "\n\n" +
                    "Its vowel backness is front, which means the tongue is positioned forward in the mouth without creating a constriction that would be classified as a consonant." +
                    "\n\n" + "It is unrounded, which means that the lips are not rounded."
            } else if (obj.title == "close-front-2") {
                this.title = "y";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Close_front_rounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is close, also known as high, which means the tongue is positioned close to the roof of the mouth without creating a constriction that would be classified as a consonant." +
                    "\n\n" +
                    "Its vowel backness is front, which means the tongue is positioned forward in the mouth without creating a constriction that would be classified as a consonant. Rounded front vowels are often centralized, which means that often they are in fact near-front." +
                    "\n\n" +
                    "Its roundedness is compressed, which means that the margins of the lips are tense and drawn together in such a way that the inner surfaces are not exposed."
            } else if (obj.title == "close-central-1") {
                this.title = "ɨ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Close_central_unrounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is close, also known as high, which means the tongue is positioned close to the roof of the mouth without creating a constriction that would be classified as a consonant." +
                    "\n\n" +
                    "Its vowel backness is central, which means the tongue is positioned halfway between a front vowel and a back vowel." +
                    "\n\n" + "It is unrounded, which means that the lips are not rounded."
            } else if (obj.title == "close-central-2") {
                this.title = "ʉ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Close_central_rounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is close, also known as high, which means the tongue is positioned close to the roof of the mouth without creating a constriction that would be classified as a consonant." +
                    "\n\n" +
                    "Its vowel backness is central, which means the tongue is positioned halfway between a front vowel and a back vowel." +
                    "\n\n" +
                    "Its roundedness is protruded, which means that the corners of the lips are drawn together, and the inner surfaces exposed."
            } else if (obj.title == "close-back-1") {
                this.title = "ɯ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Close_back_unrounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is close, also known as high, which means the tongue is positioned close to the roof of the mouth without creating a constriction that would be classified as a consonant." +
                    "\n\n" +
                    "Its vowel backness is back, which means the tongue is positioned back in the mouth without creating a constriction that would be classified as a consonant. Unrounded back vowels tend to be centralized, which means that often they are in fact near-back." +
                    "\n\n" + "It is unrounded, which means that the lips are not rounded."
            } else if (obj.title == "close-back-2") {
                this.title = "u";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Close_back_rounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is close, also known as high, which means the tongue is positioned close to the roof of the mouth without creating a constriction that would be classified as a consonant." +
                    "\n\n" +
                    "Its vowel backness is back, which means the tongue is positioned back in the mouth without creating a constriction that would be classified as a consonant." +
                    "\n\n" +
                    "Its roundedness is protruded, which means that the corners of the lips are drawn together, and the inner surfaces exposed."
            } else if (obj.title == "near-close-near-front-1") {
                this.title = "ɪ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Near-close_near-front_unrounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is near-close, also known as near-high, which means the tongue is not quite so constricted as a close vowel (high vowel)." +
                    "\n\n" +
                    "Its vowel backness is front, which means the tongue is positioned forward in the mouth without creating a constriction that would be classified as a consonant." +
                    "\n\n" + "It is unrounded, which means that the lips are not rounded."
            } else if (obj.title == "near-close-near-front-2") {
                this.title = "ʏ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Near-close_near-front_rounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is near-close, also known as near-high, which means the tongue is not quite so constricted as a close vowel (high vowel)." +
                    "\n\n" +
                    "Its vowel backness is front, which means the tongue is positioned forward in the mouth without creating a constriction that would be classified as a consonant. Rounded front vowels are often centralized, which means that often they are in fact near-front." +
                    "\n\n" +
                    "Its roundedness is compressed, which means that the margins of the lips are tense and drawn together in such a way that the inner surfaces are not exposed. The prototypical [ʏ] has a weak compressed rounding, more like [œ] than the neighboring cardinal vowels."
            } else if (obj.title == "near-close-near-back-1") {
                this.title = "ʊ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Near-close_near-back_rounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is near-close, also known as near-high, which means the tongue is not quite so constricted as a close vowel (high vowel)." +
                    "\n\n" +
                    "Its vowel backness is back, which means the tongue is positioned back in the mouth without creating a constriction that would be classified as a consonant." +
                    "\n\n" +
                    "Its roundedness is protruded, which means that the corners of the lips are drawn together, and the inner surfaces exposed. The prototypical [ʊ] has a weak protruded rounding, more like [ɔ] than the neighboring cardinal vowels."
            } else if (obj.title == "close-mid-front-1") {
                this.title = "e";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Close-mid_front_unrounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is close-mid, also known as high-mid, which means the tongue is positioned halfway between a close vowel (a high vowel) and a mid vowel." +
                    "\n\n" +
                    "Its vowel backness is front, which means the tongue is positioned forward in the mouth without creating a constriction that would be classified as a consonant." +
                    "\n\n" + "It is unrounded, which means that the lips are not rounded."
            } else if (obj.title == "close-mid-near-front-1") {
                this.title = "ø";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Close-mid_front_rounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is close-mid, also known as high-mid, which means the tongue is positioned halfway between a close vowel (a high vowel) and a mid vowel." +
                    "\n\n" +
                    "Its vowel backness is front, which means the tongue is positioned forward in the mouth without creating a constriction that would be classified as a consonant. Rounded front vowels are often centralized, which means that often they are in fact near-front." +
                    "\n\n" +
                    "Its roundedness is compressed, which means that the margins of the lips are tense and drawn together in such a way that the inner surfaces are not exposed."
            } else if (obj.title == "close-mid-central-1") {
                this.title = "ɘ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Close-mid_central_unrounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is close-mid, also known as high-mid, which means the tongue is positioned halfway between a close vowel (a high vowel) and a mid vowel." +
                    "\n\n" +
                    "Its vowel backness is central, which means the tongue is positioned halfway between a front vowel and a back vowel." +
                    "\n\n" + "It is unrounded, which means that the lips are not rounded."
            } else if (obj.title == "close-mid-near-back-1") {
                this.title = "ɵ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Close-mid_central_rounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is close-mid, also known as high-mid, which means the tongue is positioned halfway between a close vowel (a high vowel) and a mid vowel." +
                    "\n\n" +
                    "Its vowel backness is central, which means the tongue is positioned halfway between a front vowel and a back vowel." +
                    "\n\n" +
                    "Its roundedness is protruded, which means that the corners of the lips are drawn together, and the inner surfaces exposed."
            } else if (obj.title == "close-mid-back-1") {
                this.title = "ɤ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Close-mid_back_unrounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is close-mid, also known as high-mid, which means the tongue is positioned halfway between a close vowel (a high vowel) and a mid vowel." +
                    "\n\n" +
                    "Its vowel backness is back, which means the tongue is positioned back in the mouth without creating a constriction that would be classified as a consonant. Unrounded back vowels tend to be centralized, which means that often they are in fact near-back." +
                    "\n\n" + "It is unrounded, which means that the lips are not rounded."
            } else if (obj.title == "close-mid-back-2") {
                this.title = "o";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Close-mid_back_rounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is close-mid, also known as high-mid, which means the tongue is positioned halfway between a close vowel (a high vowel) and a mid vowel." +
                    "\n\n" +
                    "Its vowel backness is back, which means the tongue is positioned back in the mouth without creating a constriction that would be classified as a consonant." +
                    "\n\n" +
                    "Its roundedness is protruded, which means that the corners of the lips are drawn together, and the inner surfaces exposed."
            } else if (obj.title == "mid-central-1") {
                this.title = "ə";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Mid-central_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is mid, which means the tongue is positioned halfway between a close vowel and an open vowel." +
                    "\n\n" +
                    "Its vowel backness is central, which means the tongue is positioned halfway between a front vowel and a back vowel." +
                    "\n\n" + "It is unrounded, which means that the lips are not rounded."
            } else if (obj.title == "open-mid-near-front-1") {
                this.title = "ɛ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Open-mid_front_unrounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is open-mid, also known as low-mid, which means the tongue is positioned halfway between an open vowel (a low vowel) and a mid vowel." +
                    "\n\n" +
                    "Its vowel backness is front, which means the tongue is positioned forward in the mouth without creating a constriction that would be classified as a consonant." +
                    "\n\n" + "It is unrounded, which means that the lips are not rounded."
            } else if (obj.title == "open-mid-central-1") {
                this.title = "œ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Open-mid_front_rounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is open-mid, also known as low-mid, which means the tongue is positioned halfway between an open vowel (a low vowel) and a mid vowel." +
                    "\n\n" +
                    "Its vowel backness is front, which means the tongue is positioned forward in the mouth without creating a constriction that would be classified as a consonant. Rounded front vowels are often centralized, which means that often they are in fact near-front." +
                    "\n\n" +
                    "Its roundedness is compressed, which means that the margins of the lips are tense and drawn together in such a way that the inner surfaces are not exposed."
            } else if (obj.title == "open-mid-central-2") {
                this.title = "ɜ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Open-mid_central_unrounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is open-mid, also known as low-mid, which means the tongue is positioned halfway between an open vowel (a low vowel) and a mid vowel." +
                    "\n\n" +
                    "Its vowel backness is central, which means the tongue is positioned halfway between a front vowel and a back vowel." +
                    "\n\n" + "It is unrounded, which means that the lips are not rounded."
            } else if (obj.title == "open-mid-near-back-1") {
                this.title = "ɞ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Open-mid_central_rounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is open-mid, also known as low-mid, which means the tongue is positioned halfway between an open vowel (a low vowel) and a mid vowel." +
                    "\n\n" +
                    "Its vowel backness is central, which means the tongue is positioned halfway between a front vowel and a back vowel." +
                    "\n\n" + "It is rounded, which means that the lips are rounded rather than spread or relaxed."
            } else if (obj.title == "open-mid-back-1") {
                this.title = "ʌ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Open-mid_back_unrounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is open-mid, also known as low-mid, which means the tongue is positioned halfway between an open vowel (a low vowel) and a mid vowel." +
                    "\n\n" +
                    "Its vowel backness is back, which means the tongue is positioned back in the mouth without creating a constriction that would be classified as a consonant. Unrounded back vowels tend to be centralized, which means that often they are in fact near-back." +
                    "\n\n" + "It is unrounded, which means that the lips are not rounded."
            } else if (obj.title == "open-mid-back-2") {
                this.title = "ɔ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Open-mid_back_rounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is open-mid, also known as low-mid, which means the tongue is positioned halfway between an open vowel (a low vowel) and a mid vowel." +
                    "\n\n" +
                    "Its vowel backness is back, which means the tongue is positioned back in the mouth without creating a constriction that would be classified as a consonant." +
                    "\n\n" +
                    "Its roundedness is protruded, which means that the corners of the lips are drawn together, and the inner surfaces exposed."
            } else if (obj.title == "near-open-near-front-1") {
                this.title = "æ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Near-open_front_unrounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is near-open, also known as near-low, which means the tongue is positioned similarly to an open vowel, but is slightly more constricted – that is, the tongue is positioned similarly to a low vowel, but slightly higher." +
                    "\n\n" +
                    "Its vowel backness is front, which means the tongue is positioned forward in the mouth without creating a constriction that would be classified as a consonant." +
                    "\n\n" + "It is unrounded, which means that the lips are not rounded."
            } else if (obj.title == "near-open-near-back-1") {
                this.title = "ɐ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Near-open_central_unrounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is open, also known as low, which means the tongue is positioned far from the roof of the mouth – that is, low in the mouth." +
                    "\n\n" +
                    "Its vowel backness is front, which means the tongue is positioned forward in the mouth without creating a constriction that would be classified as a consonant. This subsumes central open (central low) vowels because the tongue does not have as much flexibility in positioning as it does in the mid and close (high) vowels; the difference between an open front vowel and an open back vowel is similar to the difference between a close front and a close central vowel, or a close central and a close back vowel." +
                    "\n\n" + "It is unrounded, which means that the lips are not rounded."
            } else if (obj.title == "open-central-1") {
                this.title = "a";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Open_front_unrounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is open, also known as low, which means the tongue is positioned far from the roof of the mouth – that is, low in the mouth." +
                    "\n\n" +
                    "Its vowel backness is front, which means the tongue is positioned forward in the mouth without creating a constriction that would be classified as a consonant. Rounded front vowels are often centralized, which means that often they are in fact near-front." +
                    "\n\n" + "It is rounded, which means that the lips are rounded rather than spread or relaxed."
            } else if (obj.title == "open-near-back-1") {
                this.title = "ä";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Open_front_rounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is open, also known as low, which means the tongue is positioned far from the roof of the mouth – that is, low in the mouth." +
                    "\n\n" +
                    "Its vowel backness is central, which means the tongue is positioned halfway between a front vowel and a back vowel. This often subsumes open (low) front vowels, because the tongue does not have as much flexibility in positioning as it does for the close (high) vowels; the difference between an open front vowel and an open back vowel is equal to the difference between a close front and a close central vowel, or a close central and a close back vowel." +
                    "\n\n" + "It is unrounded, which means that the lips are not rounded."
            } else if (obj.title == "open-back-1") {
                this.title = "ɑ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Open_back_unrounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is open, also known as low, which means the tongue is positioned far from the roof of the mouth – that is, low in the mouth." +
                    "\n\n" +
                    "Its vowel backness is back, which means the tongue is positioned back in the mouth without creating a constriction that would be classified as a consonant. Unrounded back vowels tend to be centralized, which means that often they are in fact near-back." +
                    "\n\n" + "It is unrounded, which means that the lips are not rounded."
            } else if (obj.title == "open-back-2") {
                this.title = "ɒ";
                this.audioURL = "https://www.internationalphoneticalphabet.org/ipa-chart-audio/mp3/Open_back_rounded_vowel.mp3";
                this.feature =
                    "\n\n" +
                    "Its vowel height is open, also known as low, which means the tongue is positioned far from the roof of the mouth – that is, low in the mouth." +
                    "\n\n" +
                    "Its vowel backness is back, which means the tongue is positioned back in the mouth without creating a constriction that would be classified as a consonant." +
                    "\n\n" + "It is rounded, which means that the lips are rounded rather than spread or relaxed."
            }
        },
        methods: {
            playAudio: function() {
                var innerAudioContext = uni.createInnerAudioContext();
                innerAudioContext.src = this.audioURL;
                innerAudioContext.play();
            }
        }
    }
</script>

<style>
    @import url("@/static/text.css");

    .title-button-area {
        display: flex;
        flex-direction: raw;
        justify-content: flex-start;
        align-items: center;
        text-align: center;
        width: 100vw;
        background-color: #FFFFD7;
    }

    .this-title {
        font-size: xx-large;
        font-family: serif;
        color: #3C3C3C;
        margin-top: 2.5%;
        margin-bottom: 5%;
        margin-left: 2.5%;
        margin-right: 2.5%;
    }

    .play-button {
        width: 48rpx;
        height: 48rpx;
        margin-top: 2.5%;
        margin-bottom: 5%;
        margin-left: 2.5%;
        margin-right: 2.5%;
        background-color: #FFFFFF;
    }
</style>
