<template>
    <div class="Mailchimp">
        <div class="Mailchimp-message" v-show="message !== null">{{ message }}</div>
        <form action="#" class="Mailchimp-form" v-on:submit.prevent="submitForm()">
            <input type="text" class="Mailchimp-input" placeholder="Renseignez votre email">
            <button type="submit" class="Mailchimp-submit"></button>
        </form>
    </div>
</template>

<script>
    export default {
        data () {
            return {
                message: null
            };
        },
        props: {
            success: {
                type: String,
                default: 'Vous êtes désormais inscrit, merci !'
            },
            error: {
                type: String,
                default: 'Erreur lors de votre inscription'
            },
            placeholder: {
                type: String,
                default: 'Renseignez votre email'
            },
            id: {
                type: String,
                default: ''
            },
        },
        mounted() {

        },
        methods: {
            submitForm() {
                this.message = this.success
            }
        }
    }
</script>

<style scoped>
    .Mailchimp{
        box-sizing: border-box;
    }
    .Mailchimp-input{
        box-sizing: border-box;
        position: relative;
        width: 100%;
        height: 60px;
        display: block;
        padding: 0;
        border: 1px solid rgba(0,0,0,0.2);
        border-radius: 50px;
        outline: none !important;
        padding: 0 20px;
        font-size: 22px;
    }
    .Mailchimp-input:focus{
        border-color: rgba(0,0,0,0.4);
    }
    .Mailchimp-form{
        height: 60px;
        width: 100%;
        position: relative;
    }
    .Mailchimp-submit{
        position: absolute;
        right: 9px; top: 10px;
        height: 42px; width: 42px;
        display: block;
        border: 1px solid rgba(0,0,0,0.2);
        border-radius: 50px;
    }
    .Mailchimp-message{
        padding: 10px;
        text-align: center;
    }
</style>