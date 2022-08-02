<template>
<section class="build">
  <h2>Ready To Build Your Community?</h2>
  <a id="getStartedFree" href="#">Get Started For Free</a>
</section>
</template>


<style scoped>

.build {
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: center;
  gap:2em;
  margin-bottom: 15em;
}

.build h2 {
  font-size: 2em;
  font-family: var(--poppins);
  font-weight: var(--700);
}
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