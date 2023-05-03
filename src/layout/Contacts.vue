<template>
    <div class="contacts">
        <div class="contacts_info">
            <img class="contacts_info_img" src="/src/assets/img/avatar.png" alt="avatar">
            <div class="contacts_info_wrap">
            <h3 class="contacts_info_title">Ricardo Cooper</h3>
            </div>
        </div>
        <div class="contacts_message">
            <a class="contacts_message_link" :href="`mailto:${mail}`">
            <img src="/src/assets/img/mail.svg" alt="mail">
            <p>Message</p>
            </a>
            <a class="contacts_message_link" :href="`tel:${phone}`">
                <img src="/src/assets/img/phone.svg" alt="phone">
                <p>Call</p>
            </a>
        </div>
        
    </div>
</template>
<script>
export default {
    props:{
        mail:{
            type: String,
            requred: true
        },
        phone:{
            type: String,
            requred: true
        }
    }
    
}
</script>
<style lang="scss" scoped>
.contacts{
    display: flex;
    justify-content: space-between;
    max-width: 960px;
    margin: auto;
    &_info{
        display: flex;
        align-items: end;
        &_img{
            border-radius: 50%;
            width: 128px;
            height: 128px;
        }
        &_wrap{
            height: 38px;
            display: flex;
            align-items: center;
            margin-bottom: 7px;
            .contacts_info_title{
                font-family: 'Inter';
                font-style: normal;
                font-weight: 700;
                font-size: 24px;
                line-height: 32px;
                color: #111827;
            }
        }
    }
    &_message{
        display: flex;
        gap: 16px;
        align-items: flex-end;
        &_link{
        height: 38px;
        text-decoration: none;
        height: fit-content;
        display: flex;
        gap: 10px;
        background: #FFFFFF;
        border: 1px solid #D1D5DB;
        box-shadow: 0px 1px 2px rgba(0, 0, 0, 0.05);
        border-radius: 6px;
        padding: 8px 17px 8px 13px;
        margin-bottom: 7px;
        p {
            font-family: 'Inter';
            font-style: normal;
            font-weight: 500;
            font-size: 14px;
            line-height: 20px;
            color: #374151;
        }
        }
    }
}
</style>