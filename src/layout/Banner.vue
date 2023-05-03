<template>
        <div :style=" {'background-image': 'url(' + img + ')'} " class="banner">
            
        </div>
</template>
<script>
export default {
    props: {
        img:{
            type: String,
            required: true
        }
    }
    
}
</script>
<style lang="scss" scoped>
.banner{
    height: 192px;
}
</style>