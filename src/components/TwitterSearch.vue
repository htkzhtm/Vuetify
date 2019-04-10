<template>
    
</template>

<script lang="ts">
import Vue from 'vue';
import dotenv from 'dotenv';
dotenv.config()
const Twitter = require('twitter')

const consumerKey = process.env.VUE_APP_TWITTER_CLIENT_KEY
const consumerSecret = process.env.VUE_APP_TWITTER_CLIENT_SECRET
const accessTokenKey = process.env.VUE_APP_ACCESS_TOKEN
const accessTokenSecret = process.env.VUE_APP_ACCESS_TOKEN_SECRET

const client = new Twitter({
  consumerKey,
  consumerSecret,
  accessTokenKey,
  accessTokenSecret
})
export default Vue.extend({
    created () {
        const params = {count: 50};
        client.get('statuses/home_timeline', params, function(error: any, tweets: any, response: any) {
            if (!error) {
                console.log(tweets)
            }
            console.log(tweets)
        });
    }
});
</script>
