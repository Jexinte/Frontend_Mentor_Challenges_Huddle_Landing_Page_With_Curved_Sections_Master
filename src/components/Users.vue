<template>
  <section class="users">
    <div class="left-users">
      <h2>Your Users</h2>
      <p>It takes no time at all to integrate Huddle with your app's authentication solution. This means, once signed in to your app, your users can start chatting immediately.</p>
    </div>

    <div class="right-users">
      <img src="@/assets/images/illustration-your-users.svg" alt="Users illustrations">
    </div>
  </section>
</template>


<style scoped>

.users {
  display: flex;
  position: relative;
  padding-inline:2em;
  gap:2em;
  padding-top: 5em;
  padding-bottom: 5em;
   background-color: var(--veryPaleBlue); 
}

.left-users {
  display: flex;
  flex-direction: column;
  gap:1.5em;
  justify-content: center;

}

.left-users h2 {
  font-family: var(--poppins);
  font-weight: var(--700);
  font-size: 2em;
}
.left-users p {
  font-family: var(--openSans);
  font-weight: var(--400);
  width: 514px;
}



.right-users img {
  width: 100%;
}


.users::before {
  content:'';
  position: absolute;
  background-image: url('../assets/images/bg-section-top-desktop-2.svg');
  background-repeat: no-repeat;
  background-size: 100%;
  top:0;
  left:0;
  bottom:0;
  right:0;
}

.users::after {
  content:'';
  position: absolute;
  background-image: url('../assets/images/bg-section-bottom-desktop-2.svg');
  background-repeat: no-repeat;
  background-size: 100%;
   top:0; 
  left:0;
  bottom:0;
  right:0;
  transform: translateY(100%);
}




@media screen and (min-width:993px) and (max-width:1135px) {
  
  .users::before {
    transition : transform 500ms ease-out;
    transform : translateY(-22%)
  }
}

@media screen and (min-width:1136px) and (max-width:1399px) {
  
  .users::before {
    transition : transform 500ms ease-out;
    transform : translateY(-20%)
  }
}

@media screen and (min-width:1399px) and (max-width:1617px){
  
  .users::before {
    transition : transform 500ms ease-out;
    transform : translateY(-19%)
  }
}


@media screen and (min-width:1618px) and (max-width:1820px){
  
  .users::before {
    transition : transform 500ms ease-out;
    transform : translateY(-18%)
  }
}



@media screen and (min-width:1821px){
  
  .users::before {
    transition : transform 500ms ease-out;
    transform : translateY(-19%)
  }
}

/* MOBILE */

@media screen and (max-width:992px) {
  .users{
    flex-direction: column;
    text-align: center;
    gap: 2em;
  }

  .left-users p {
    width: 100%;
  }

  .right-users {
    order:-1;
  }

  .users::after {
  background-image: url('../assets/images/bg-section-bottom-mobile-2.svg');
  
}
 .users::before {
  background-image: url('../assets/images/bg-section-top-mobile-2.svg');
}
}

@media screen and (min-width:874px) and (max-width:992px) {
   .users::before {
     transform: translateY(-26%);
}

}


@media screen and (min-width:766px) and (max-width:874px) {
   .users::before {
  transform: translateY(-25%);
}


}


@media screen and (min-width:676px) and (max-width:765px) {
   .users::before {
  transform: translateY(-24%);
}

}


 @media screen  and (min-width:578px) and (max-width:675px) {
   .users::before {
  transform: translateY(-22%);
}

} 


 @media screen  and (min-width:516px) and (max-width:674px) {
   .users::before {
  transform: translateY(-21%);
}

} 


 @media screen  and (min-width:475px) and (max-width:515px) {
   .users::before {
  transform: translateY(-19.5%);
}

} 

</style>