# WIP do not use
# 221-vue-mailchimp

Mailchimp component for VueJS


## Installation

```
npm install 221-vue-mailchimp --save
```

## Usage

```
<template>
  <div id="myapp">
    <mailchimp
      :success="'Vous êtes désormais inscrit, merci !'"
      :error="'Erreur lors de votre inscription'"
      :placeholder="'Renseignez votre email'"
      :url="'http://growdc.us14.list-manage.com/subscribe/post?u=6c5bd30569b03c131ce559daf&id=8dea76fc1c'"
    ></mailchimp>
  </div>
</template>
```

```
import Mailchimp from 'vue-web-cam/src/Mailchimp'

export default {
  components: {
    Mailchimp
  }
}
```

