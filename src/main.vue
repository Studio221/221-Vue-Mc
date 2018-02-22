<template>
  <div id="app" class="component">
    <mailchimp
      :success="'Vous êtes désormais inscrit, merci !'"
      :error="'Erreur lors de votre inscription'"
      :placeholder="'Renseignez votre email'"
      :url="'http://growdc.us14.list-manage.com/subscribe/post?u=6c5bd30569b03c131ce559daf&id=8dea76fc1c'"
    ></mailchimp>
  </div>
</template>

<script>
  import Mailchimp from './Mailchimp'

  export default {
    name: 'app',
    data() {
        return {};
    },
    methods: {},
    components: {
      Mailchimp
    }
  }
</script>
