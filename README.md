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
      :id="'ZAEH907'"
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

