<template>
 <section class="flowingConversations">
  <div class="left-illustration">
    <img src="@/assets/images/illustration-flowing-conversation.svg" alt="Illustration people talking">
  </div>

  <div class="right">
    <h2>Flowing Conversations</h2>
    <p>You would'nt paginate a conversation in real life, so why do it online ? Our threads have just-in-time loading for a more natural flow.</p>
  </div>
 </section> 
</template>

<style scoped>

.flowingConversations {
  display: flex;
  gap: 2em;
}

.left-illustration img {
  width: 100%;
}

.right {
  display: flex;
  flex-direction: column;
  justify-content: center;
  gap: 1.5em;
  padding-inline: 2em;
}
.right h2 {
  font-family: var(--poppins);
  font-weight: var(--700);
  font-size: 2em;
}

.right p {
  font-family: var(--openSans);
  font-weight: var(--400);
  width: 505px;
}
</style>