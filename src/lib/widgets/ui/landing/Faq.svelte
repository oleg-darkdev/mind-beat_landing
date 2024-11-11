<script>
  import {faq} from '$shared';
</script>

<section class="section_sponsor">
  <div class="padding-global padding-section-medium">
    <a name="faq"></a>


  <h2  class="heading text-center">F.A.Q.</h2>
    <div class="spacer-large"></div>


    <div class="max-w-4xl mx-auto">
      {#each faq as question}
      <button on:click={()=> question.showAnswer = !question.showAnswer} class="big-btn mb-4">
        <div class='flex flex-row justify-between w-full items-center content-center'>
          <h3 class="text-size-large">{question.q}?</h3>
          <div class="icon-embed-faq w-embed">
            <img src="{question.showAnswer ? '/images/arrow-up.svg': '/images/arrow-down.svg'}" class='' alt="">
          </div>
        </div>
        <div class="wp2024-overlay"></div>
          {#if question.showAnswer}
          <div class="flex flex-col items-start">
            {#each question.a as answer}
              <p class="text-size-medium leading-relaxed mb-4">
                {answer}
              </p>
            {/each}
            </div>
          {/if}

      </button>


      {/each}
    </div>
  </div>
</section>


<style>
.icon-embed-faq {
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 4rem;
  height: 4rem;
  display: flex;
}


.inscription_component .icon-embed-faq,
.big-btn .icon-embed-faq {
  position: relative;
  z-index: 0;
  top: 0rem;
  right: 0rem;
  transition: top 200ms ease, right 200ms ease;
}

.inscription_component:hover .icon-embed-faq,
.big-btn:hover .icon-embed-faq {
  top: -0.5rem;
  right: -0.5rem;
}


.big-btn {
  z-index: 1;
  grid-column-gap: 1rem;
  border: 1px solid var(--wp-2024--blue);
  text-align: left;
  background-color: #146ef51f;
  border-radius: 0.25rem;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  padding: 2rem;
  display: flex;
  position: relative;
}

@media screen and (max-width: 767px) {
  .big-btn {
    flex-direction: column;
  }
}

@media screen and (max-width: 479px) {
  .big-btn {
    padding: 1.25rem;
  }
}
</style>
