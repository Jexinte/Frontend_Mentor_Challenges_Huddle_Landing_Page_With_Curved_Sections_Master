<template>
<a id="getStartedFree" href="#">Get Started For Free</a>
</template>

<style scoped>

#getStartedFree:visited {
  color:var(--white)
}
#getStartedFree {
background: var(--pink);
color: var(--white);
margin: 0 auto;
padding: 19px 60px 20px;
border-radius: 50px;
font-weight: var(--700);
box-shadow: -3px 5px 10px rgba(0,0,0,0.2);
position: relative;
  margin-bottom: 45px;
}

#getStartedFree::after {
  content: '';
  position: absolute;
  top:0;
  bottom:0;
  right:0;
  left:0;  
padding: 19px 60px 20px;
border-radius: 50px;
  display: block;
}

#getStartedFree:hover::after {
  opacity: .5;
  background-color:white;

}


</style>