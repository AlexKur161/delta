<template>
    <div class="container">
        <Banner
        img="/src/assets/img/bg.png"
        />
        <Contacts
        mail="AlexKur-web@yandex.ru"
        phone="83673737383"
        />
        <PictureFeed />
    </div>
</template>
<script>
import Banner from "../layout/Banner.vue"
import Contacts from "../layout/Contacts.vue"
import PictureFeed from "../components/PictureFeed.vue"
export default {
    data(){
        return {

        }
    },
    components: {
        Banner,
        Contacts,
        PictureFeed
    }
}
</script>