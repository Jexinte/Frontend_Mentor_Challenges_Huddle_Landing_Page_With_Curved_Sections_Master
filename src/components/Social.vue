<template>
<footer class="social">

    <div class="left-social">
      
      <img id="logo" src="@/assets/images/logo-copy.svg" alt="Logo">
          <p id="social-paragraph-below-logo">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris nulla quam, hendrerit lacinia vestibulum a , ultrices quis sem</p>

          <div class="phone-contact box">
            
            <img src="@/assets/images/icon-phone.svg" alt="Icon phone">
            <p>Phone: +1-543-123-4567</p>

          </div>

          <div class="email-contact box" id="emailContact">
            
            <img src="@/assets/images/icon-email.svg" alt="Icon emaim">
            <p>example@huddle.com</p>

          </div>

          <div class="social-icons">
            
            <font-awesome-icon icon="fa-brands fa-square-facebook" class="fa-brands" id="facebook" />
            <font-awesome-icon icon="fa-brands fa-instagram" class="fa-brands" id="instagram" />
            <font-awesome-icon icon="fa-brands fa-square-twitter" class="fa-brands" id="twitter" />

          </div>
    </div>

    <div class="right-social">
      <div class="newsletter-introduction">
        <h3>NEWSLETTER</h3>
        <p>To receive tips on how to grow your community, sign up to our weekly newsletter. We'll never send you spam or pass on your email address </p>
      </div>

      <form>
        <input type="email" id="mail">
        <p id="errormsg"> Check your email please</p>
        <input id="submit" type="submit" value="Suscribe">
      </form>
    </div>

  </footer>
</template>

<script>
  export default {
    

    mounted:function(){
      this.checkingEmailFormat()
    },
    methods: {
      checkingEmailFormat() {
        const form = document.querySelector('form')
        form.addEventListener('submit',(e) => {
           e.preventDefault()
      
          const errorMsgHidden = document.getElementById('errormsg')
          const mail = document.getElementById('mail')
          let regexMail = new RegExp(/^[a-z0-9._-]+@[a-z0-9._-]{2,}\.[a-z]{2,4}$/)
            if(!regexMail.test(mail.value)) {
              errorMsgHidden.style.display = "block"
              mail.style.border ="1px solid red"
            }
           else if(regexMail.test(mail.value)){
             alert('Your email have been send !')
            errorMsgHidden.style.display = "none"
            mail.style.border ="1px solid lightgray" 
           }
          
        })
      }
    }
  }
</script>
<style scoped>

#errormsg{
  position: absolute;
  font-size: .8em;
  top:45px;
  display: none;
  color:red;
}
.social {
  display: flex;
  padding-inline: 64px;
  background-color: var(--veryDarkCyan);
  position: relative;
  padding-bottom: 10em;
}

  .social::before {
  content:'';
  position: absolute;
  background-image: url('../assets/images/bg-footer-top-desktop.svg');
  background-repeat: no-repeat;
  background-size: 100%;
  top:-109px;
  left:0;
  bottom:0;
  right:0;
}


.social p {
  line-height: 1.6em;
}
#logo{
  width: 246px;
}
.left-social {
  display: flex;
  flex-direction: column;
  gap:1em;
  width: 50%;
position: relative;
}

.left-social p {
  font-family: var(--openSans);
  font-weight: var(--400);
  color:white;
}

.phone-contact {
  display: flex;
}
.email-contact {
  display: flex;
}
.right-social {
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 50%;
  position: relative;
}

#social-paragraph-below-logo{
position: relative;
bottom: 90px;
width: 337px;
font-size: .9em;
}

.email-contact p {
  position: relative;
  right:5px;
}

#emailContact{
  position: relative;
  top:-70px;
  
}
.box{
  gap: 1em;
position: relative;
bottom: 5em;
}

.box img {
  height: 20px;
}

.social-icons {
  font-size: 2em;
  display: flex;
  gap:.8em;
  position: relative;
}

.fa-brands {
  font-size: 1.12em;
  cursor: pointer;
  color:white;
}

#twitter:hover{
  color:#00CBFA;
}

form {
  display: flex;
  position: relative;
}

.newsletter-introduction p {
  font-size: .9em;
  font-family: var(--openSans);
  font-weight: var(--400);
position: relative;
bottom: 26px;
color: white;
width: 353px;
}

.newsletter-introduction h3 {
  position: relative;
  bottom: 50px;
  font-size: 1.5em;
  font-family: var(--poppins);
  font-weight: var(--700);
  color:white;
}

#submit {
  padding: .7em 4em;
  width: 100%;
  background-color:var(--pink);
  border:none;
  border-radius: 5px;
  font-family: var(--poppins);
  font-weight: var(--700);
  color:white;
  cursor: pointer;
  position: relative;
}
#submit::after {
  content: '';
  position: absolute;
  top:0;
  bottom:0;
  right:0;
  left:0;
  padding: .7em 4em;
  background-color: rebeccapurple;
  z-index: 9999;
}


input[type="email"]{
  width: 100%;
  cursor: pointer;
}

form {
  gap:1em;
}
 /* DEKSTOP MEDIA QUERIES */
@media screen and (min-width:1055px) and (max-width:1109px) {
  
  .social::before {
    transition : top 300ms ease-in;
    top:-115px;
  }
}

@media screen and (min-width:1110px) and (max-width:1169px)  {
  
  .social::before {
    transition : top 300ms ease-in;
    top:-121px;
  }
}



@media screen and (min-width:1170px) and (max-width:1227px)  {
  
  .social::before {
    transition : top 300ms ease-in;
    top:-128px;
  }
}


@media screen and (min-width:1227px) and (max-width:1308px)  {
  
  .social::before {
    transition : top 300ms ease-in;
    top:-135px;
  }
}


@media screen and (min-width:1308px) and (max-width:1385px)  {
  
  .social::before {
    transition : top 300ms ease-in;
    top:-143px;
  }
}

@media screen and (min-width:1386px) and (max-width:1468px)  {
  
  .social::before {
    transition : top 300ms ease-in;
    top:-152px;
  }
}

@media screen and (min-width:1469px) and (max-width:1555px)  {
  
  .social::before {
    transition : top 300ms ease-in;
    top:-161px;
  }
}


@media screen and (min-width:1556px) and (max-width:1645px)  {
  
  .social::before {
    transition : top 300ms ease-in;
    top:-170px;
  }
}


@media screen and (min-width:1556px) and (max-width:1645px)  {
  
  .social::before {
    transition : top 300ms ease-in;
    top:-170px;
  }
}

@media screen and (min-width:1646px) and (max-width:1737px)  {
  
  .social::before {
    transition : top 300ms ease-in;
    top:-180px;
  }
}



@media screen and (min-width:1738px) and (max-width:1833px)  {
  
  .social::before {
    transition : top 300ms ease-in;
    top:-190px;
  }
}


@media screen and (min-width:1834px)  {
  
  .social::before {
    transition : top 300ms ease-in;
    top:-201px;
  }
}

/* MOBILE  */

@media screen and (max-width:992px) {
  .social{
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-top:6em;
  }

.social::before {
  content:'';
  background-image: url('../assets/images/bg-footer-top-mobile.svg');
 }

  
  .right-social {
    order:-1;
    width: 100%;
    position: relative;
    z-index: 9999;
  }

  form {
    display: flex;
    flex-direction: column;
  }

  .left-social {
    display: flex;
    flex-direction: column;
    width: 100%;
  }
  #submit {
    width: 50%;
    position: absolute;
    right: 0;
    top:40px;
  }

  input[type="email"] {
    cursor: pointer;
padding: 6px;
border-radius: 4px;
border: none;
width:100%;
  }
}

@media screen and (min-width:770px) and (max-width:992px) {
  .social::before{
    transition : top 300ms ease-out;
    top:-109px;
  }
}

@media screen and (min-width:563px) and (max-width:769px) {
  .social::before{
    transition : top 300ms ease-out;
    top:-80px;
  }
}

@media screen and (min-width:475px) and (max-width:562px) {
  .social::before{
    transition : top 300ms ease-out;
    top:-59px;
  }
}
</style>