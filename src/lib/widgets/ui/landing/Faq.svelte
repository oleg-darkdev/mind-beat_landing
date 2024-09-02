<script>
// import {} from '$entities';

const faq = [
  {
    q: `Lorem Ipsum has been the industry's.`,
    a: [
      `Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.`,
      `It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.`,
    ]
  },
  {
    q: `Lorem Ipsum has been the industry's.`,
    a: [
      `Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.`,
      `It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.`,
    ]
  },
  {
    q: `Lorem Ipsum has been the industry's.`,
    a: [
      `Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.`,
      `It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.`,
    ]
  },
  {
    q: `Lorem Ipsum has been the industry's.`,
    a: [
      `Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.`,
      `It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.`,
    ]
  },
  {
    q: `Lorem Ipsum has been the industry's.`,
    a: [
      `Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.`,
      `It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.`,
    ]
  },
  {
    q: `Lorem Ipsum has been the industry's.`,
    a: [
      `Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.`,
      `It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.`,
    ]
  },
]
</script>

<section class="section_sponsor-wp2024">
  <div class="padding-global padding-section-medium">
  <a name="faq"></a>
  <!-- <h2  class="heading-wp2024 text-center">F.A.Q.</h2> -->
    <div class="spacer-large"></div>


    {#each faq as {q, a}}
    <button class="sponsor-wp2024_button mb-4">
      <div class="heading-wp2024">{q}?</div>
      <div class="icon-embed-faq w-embed">
        <img src="/images/arrow-down.svg" class='' alt="arrow down">
      </div>
      <div class="wp2024-overlay"></div>
    </button>
    {/each}
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


.inscription-wp2024_component .icon-embed-faq,
.sponsor-wp2024_button .icon-embed-faq {
  position: relative;
  z-index: 0;
  top: 0rem;
  right: 0rem;
  transition: top 200ms ease, right 200ms ease;
}

.inscription-wp2024_component:hover .icon-embed-faq,
.sponsor-wp2024_button:hover .icon-embed-faq {
  top: -0.5rem;
  right: -0.5rem;
}
</style>
