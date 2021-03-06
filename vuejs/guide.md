*Cai dat Vue-CLI*
B0 :
    node -v  //check version node
    npm -v   //check version npm
    npm install npm@latest -g   //update version lastest for npm

B1 : npm install -g vue-cli   //cai dat Vue-CLI
     //npm install -g @vue/cli

B2 : Tao project mau
    vue init webpack vue-cli-example

B3: DEV, Truy cap vao thu muc code, go:
    cd vue-cli-example
    npm run dev

    Build file va chay truoc khi deploy:
    npm run prod

*Keys*
- Template: 
    ref: https://bootswatch.com/cosmo/
    https://appdividend.com/2018/12/28/vue-router-tutorial-with-example-how-to-use-routing-in-vuejs/
- Vue router:
    this.$router => is the router object
    this.$route  => is the current route object

    ref: https://scotch.io/tutorials/getting-started-with-vue-router
    https://router.vuejs.org/guide/essentials/navigation.html
    https://flaviocopes.com/vue-router/
    param: https://medium.com/@saidhayani/understand-routing-in-vue-js-with-examples-6da96979c8e3
- Communication component: http://localhost:8080/user
    ref : https://viblo.asia/p/vuejs-giao-tiep-giua-cac-component-Ljy5Vxd3Zra
    + Truyen data tu componen parent xuong component child : su dung attribue props (trong component child)
    + Giao tiep component child len compoent parent
    + Giao tiep giua 2 component child co cung compoent parent
    + Giao tiep giua 2 component child khong cung component parent
    // main.js
    // Use「Vue.prototype」to setup globally
    const EventBus = new Vue()
    Object.defineProperties(Vue.prototype, {
        $bus: {
            get: function() {
                return EventBus
            }
        }
    })

    // App.vue
    // Listen the event
    this.$bus.$on('isLoading', (event) => {
        this.loadingStatus = event
    })

    // Signin.vue
    // Fire the call
    this.$bus.$emit('isLoading', false)

- Multilang :
    ref : https://viblo.asia/p/vuejs-da-ngon-ngu-trong-ung-dung-vue-6J3Zg2wLKmB
    fix lai : https://kuanhsuh.github.io/How-to-implement-multi-language-with-Vue-i18n.html
              https://github.com/kuanhsuh/vue-i18n-sandbox/blob/master/src/App.vue
    https://itnext.io/setting-language-with-i18n-by-os-language-in-vue-router-vuex-e42c9318c9ec

- VueX: Centralized State Management for Vue.js
    https://viblo.asia/p/tim-hieu-ve-vuex-6J3ZggqqZmB
    https://viblo.asia/p/gioi-thieu-ve-vuex-phan-2-924lJd7YKPM
    https://itnext.io/vuex-made-simple-getting-started-6bf229d432cf
    https://vuex.vuejs.org/guide/structure.html
    https://viblo.asia/p/vuex-va-vi-du-don-gian-GrLZDpzgZk0
    https://medium.com/dailyjs/mastering-vuex-zero-to-hero-e0ca1f421d45
    https://github.com/vanquynguyen/my-task-vuex
    https://viblo.asia/p/vuex-cho-nguoi-moi-bat-dau-4dbZNYLLKYM

- Axios Get API: là một thư viện HTTP Client dựa trên Promise
    Tim hieu them : Transforms và Interceptors
    Ref: https://viblo.asia/p/call-api-trong-vuejs-theo-cach-thong-minh-nhat-07LKXx7EKV4

- Mixin :
  https://viblo.asia/p/vuejs-tim-hieu-ve-mixins-Ljy5VLD9Zra

- Watch : https://viblo.asia/p/vue-js-thay-doi-cua-data-voi-watch-bWrZn6orZxw
    https://viblo.asia/p/vai-dieu-chua-biet-ve-watcher-trong-vuejs-3Q75wGnG5Wb

- Tham khao structure project :
    https://medium.com/hong-kong-tech/reusable-scalable-and-easy-to-organize-project-using-vuejs-part-2-c7e82044d7fc
    https://medium.com/hong-kong-tech/reusable-scalable-and-easy-to-organize-project-using-vuejs-part-3-ed8cba6b4dfe

*Deploy project vue to Heroku*
https://hoanguyenit.com/deploying-vuejs-to-heroku.html
https://medium.com/netscape/deploying-a-vue-js-2-x-app-to-heroku-in-5-steps-tutorial-a69845ace489
https://convoicoi.wordpress.com/2018/09/14/vuejs-huong-dan-deploy-vue-project-len-netlify/

*Links*
https://itnext.io/vue-js-app-performance-optimization-part-1-introduction-to-performance-optimization-and-lazy-29e4ff101019

*Login*
https://webdevchallenges.com/persist-access-token-with-vue-js/

*Authen*
https://scotch.io/tutorials/vue-authentication-and-route-handling-using-vue-router
https://scotch.io/tutorials/handling-authentication-in-vue-using-vuex

*Javascript*
https://viblo.asia/p/tu-javascript-thuan-den-rxjs-phan-1-m68Z0OJzKkG

*CRUD*
https://investmentnovel.com/vue-js-crud-example-tutorial-from-scratch/
