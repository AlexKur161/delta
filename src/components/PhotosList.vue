<template>
    <div class="container">
        <Banner
        img="/src/assets/img/bg.png"
        />
        <Contacts
        mail="AlexKur-web@yandex.ru"
        phone="83673737383"
        />
    </div>
</template>
<script>
import Banner from "../layout/Banner.vue"
import Contacts from "../layout/Contacts.vue"
export default {
    data(){
        return {

        }
    },
    components: {
        Banner,
        Contacts
    }
}
</script>