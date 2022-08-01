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
            title : 'Grow Together',
            text :`Generate meaningful discussions with your audience and build a strong, loyal community. Think of the insightful conversations you miss out on with a feedback form`
          }
        ]
      }
    }
  }
</script>

<style scoped>


/* GROWTOGETHER */

.growTogether{
display: flex;
background-color: var(--veryPaleBlue);
margin-bottom: 15em; 
position: relative;
padding-top: 5em;
padding-bottom: 5em;
}

.growTogether::before {
  content:'';
  position: absolute;
  background-image: url('../assets/images/bg-section-top-desktop-1.svg');
  background-repeat: no-repeat;
  background-size: 100%;
  top:-114px;
  left:0;
  bottom:0;
  right:0;
}

.growTogether::after {
  content:'';
  position: absolute;
  background-image: url('../assets/images/bg-section-bottom-desktop-1.svg');
  background-repeat: no-repeat;
  background-size: 100%;
   top:0; 
  left:0;
  bottom:0;
  right:0;
  transform: translateY(100%);
}
.growTogether .left {
display: flex;
padding-inline: 2em;
flex-direction: column;
gap: 1.5em;
justify-content: center;
}



.growTogether .right img {
width: 100%;
}
.growTogether .right {
padding-inline: 2em;
}



.growTogether .left h2 {
font-weight: var(--700);
font-family: var(--poppins);
font-size: 2em;
}
.growTogether .left p {
font-weight: var(--400);
font-family: var(--openSans);
}


@media screen and (min-width:475px) and (max-width:992px) {
  .growTogether::before {
  content:'';
  position: absolute;
  background-image: url('../assets/images/bg-section-top-mobile-1.svg');
  background-repeat: no-repeat;
  background-size: 100%;
  top:0;
  left:0;
  bottom:0;
  right:0;
}

.growTogether::after {
  content:'';
  position: absolute;
  background-image: url('../assets/images/bg-section-bottom-mobile-1.svg');
  background-repeat: no-repeat;
  background-size: 100%;
   top:0; 
  left:0;
  bottom:0;
  right:0;
  transform: translateY(100%);
}

.growTogether .left {
  gap:2em;
}
}

@media screen and (min-width:670px) and (max-width:992px){
  .growTogether::before {
      transform:translateY(-25%);
  }
}

@media screen and (min-width:490px) and (max-width:669px){
  .growTogether::before {
      transform:translateY(-22%);
  }
}


@media screen and (min-width:475px) and (max-width:669px){
  .growTogether::before {
      transform:translateY(-21%);
  }
}



@media screen and (min-width:1242px) and (max-width:1545px) {
  
  .growTogether::before {
    transition : top 500ms ease-out;
    top:-143px;
  }
}

@media screen and (min-width:1546px)  {
  
  .growTogether::before {
    transition : top 500ms ease-out;
    top:-177px;
  }
}

</style>