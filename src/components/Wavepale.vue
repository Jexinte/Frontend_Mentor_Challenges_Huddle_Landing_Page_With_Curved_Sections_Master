<template>
  <section class="growTogether">
    <div class="left">
      <h2 v-for="presentation in datas">{{presentation.title}}</h2>
      <p v-for="presentation in datas">{{presentation.text}}</p>
    </div>

    <div class="right">
      <img src="@/assets/images/illustration-grow-together.svg" alt="grow together image">
    </div>
  </section>
</template>

<script>
  export default {
    data(){
      return {
        datas : [{
            title : 'Your Users',
            text :`It takes no time at all to integrate Huddle with your app's authentication solution. This means, once signed in to your app, your users can start chatting immediately.`
          }
        ]
      }
    }
  }
</script>