<script setup>
    defineProps({
        previewTitle: {
            type: String,
            required: true
        },
        previewImage: {
            type: String,
            required: true
        },
        siteUrl: {
            type: String,
            required: true
        }
    })
</script>

<template>
    <a target="_blank" :href="siteUrl">
        <div class="preview">
                <div class="website-preview-img" :style="{ backgroundImage: 'url(' + previewImage + ')' }"></div>
                <div class="color-wash"></div>
                <p>{{ previewTitle }}</p>
        </div>
    </a>
</template>

<style scoped>

    .preview{
        width: 600px;
        height: 320px;
        position: relative;
        text-align: center;
        -webkit-box-shadow: 0px 0px 11px 0px rgba(0,0,0,0.75);
        -moz-box-shadow: 0px 0px 11px 0px rgba(0,0,0,0.75);
        box-shadow: 0px 0px 11px 0px rgba(0,0,0,0.75);
    }

    .website-preview-img{
        background-repeat: no-repeat;
        background-size: cover;
        position: absolute;
        height: 100%;
        width: 100%;
        top: 0;
        right: 0;
        z-index: -3;
    }
    .color-wash{
        background-color: rgba(55,55,55,0.45);
        position: absolute;
        height: 100%;
        width: 100%;
        right: 0;
        top: 0;
        z-index: -2;
        transition: background-color 0.5s
    }
    .preview p {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        transition: font-size 0.5s;
        color: white;
    }

    .preview:hover{
        font-size:1.8rem;
    }
    .preview:hover .color-wash{
        background-color: rgba(55,55,55,0.85);
    }

    @media(max-width:800px) {
        .preview{
            width: 100vw;
             height: 320px;
            position: relative;
            text-align: center;
            -webkit-box-shadow: 0px 0px 11px 0px rgba(0,0,0,0.75);
            -moz-box-shadow: 0px 0px 11px 0px rgba(0,0,0,0.75);
            box-shadow: 0px 0px 11px 0px rgba(0,0,0,0.75);
            font-size:1.8rem;
        }
        .website-preview-img{
            background-position: center; 
        }
        .color-wash{
            background-color: rgba(55,55,55,0.85);
        } 
    }
</style>