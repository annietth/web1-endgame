<template>
    <div class="container">
        <div class="container__close">
            <svg width="31" height="30" viewBox="0 0 31 30" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M0 14.7708C0 6.61313 6.83437 0 15.265 0V0C23.6956 0 30.53 6.61313 30.53 14.7708V14.7708C30.53 22.9285 23.6956 29.5417 15.265 29.5417V29.5417C6.83437 29.5417 0 22.9285 0 14.7708V14.7708Z" fill="white"/>
            <path fill-rule="evenodd" clip-rule="evenodd" d="M1.42 14.7708C1.42 22.1697 7.61862 28.1676 15.265 28.1676C22.9114 28.1676 29.11 22.1697 29.11 14.7708C29.11 7.37198 22.9114 1.37403 15.265 1.37403C7.61862 1.37403 1.42 7.37198 1.42 14.7708ZM15.265 0C6.83437 0 0 6.61313 0 14.7708C0 22.9285 6.83437 29.5417 15.265 29.5417C23.6956 29.5417 30.53 22.9285 30.53 14.7708C30.53 6.61313 23.6956 0 15.265 0Z" fill="#00A0FB"/>
            <path d="M9.01935 9.15976C9.29662 8.89146 9.74617 8.89146 10.0234 9.15976L15.6715 14.6249L21.3195 20.0901C21.5967 20.3584 21.5967 20.7934 21.3195 21.0617C21.0422 21.33 20.5927 21.33 20.3154 21.0617L9.01935 10.1313C8.74207 9.86305 8.74207 9.42805 9.01935 9.15976Z" fill="#00A0FB"/>
            <path d="M9.01935 20.8188C8.74207 20.5505 8.74207 20.1155 9.01935 19.8472L20.3154 8.91686C20.5927 8.64856 21.0422 8.64856 21.3195 8.91686C21.5967 9.18516 21.5967 9.62015 21.3195 9.88845L10.0234 20.8188C9.74617 21.0871 9.29662 21.0871 9.01935 20.8188Z" fill="#00A0FB"/>
            </svg>
        </div>
        <div class="container__texte">
            <p>{{ texte }}</p>
        </div>
    </div>
</template>
<script>
export default {
    name: 'PopUpTexte',
    props: {
        texte: String
    }
}
</script>
<style scoped lang="scss">
.container {
    @include background-boxes;
    border-radius: 0px;
    max-width: 270px;
    @include flexbox(row, flex-start, baseline);
    &__texte {
        padding: 18px;
        font-size: rem(16px);
        margin-right: 8%;
        @include tablet-up {
            font-size: rem(32px);
        }
        @include desktop-up {
            font-size: rem(40px);
        }
    }
    & path, svg {
        width: 28px;
    }
    p {
        font-size: rem($mobileP);
        color: $white;
        line-height:1.5;
    }
}

</style>