<template>
  <div id="app" class="component">
    <mailchimp
      :success="'Vous êtes désormais inscrit, merci !'"
      :error="'Erreur lors de votre inscription'"
      :placeholder="'Renseignez votre email'"
      :id="'ZAEH907'"
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
