<script>
  const organisators = [
    {
      text: 'DarkDev.Foundation',
      link: 'https://darkdev-foundation.vercel.app/',
      logo: '/images/logos/darkdev_turq.svg'
    },
    // {
    //   text: '',
    //   img: '',
    //   logo: ''
    // },
  ]
</script>

<section class="bg-[#0000]">
    <div class="padding-section-medium">
      <div class="orga-wp2024_component">

        <a name="organisators"></a>

        <div animate="from-bottom" class="heading-wp2024">Organizatorzy</div>
        <ul role="list" class="organisators-list">
          {#each organisators as {text, link, logo}}
          <li class="organisator-item">
            <a href="{link}" target="_blank" >
            <div class="h-14">
              <img src="{logo}" loading="lazy"  alt="{text} logo" class="h-full w-full">
            </div>
            </a>
          </li>
          {/each}

            <div class="grid grid-cols-2 gap-6">
              <li class="">
              <a href="https://www.facebook.com/serumgdansk/"  target="_blank"  >
                <div class="organisator-item">
                <div class="organisator_logo-wrapper">
                  <img src="/images/logos/serum.png" loading="lazy" width="200" height="200" alt="Serum Food&Drinks logo" class="organisator_logo">
                </div>

                <span class="text-weight-medium">Serum  <br/> Food&Drinks</span>
              </div>
              </a>
            </li>

            <li class="">
              <a href="https://oleg-darkdev.vercel.app/"  target="_blank"  >
                <div class="organisator-item">
                <div class="organisator_logo-wrapper">
                  <img src="/images/oleg-avatar.png" loading="lazy" width="200" height="200" alt="" class="organisator_logo">
                </div>

                <span class="text-weight-medium">Oleg <br/> Medvedev</span>
              </div>
              </a>
            </li>
          </div>


        </ul>
      </div>
    </div>
  </section>


<style>


.organisators-list {
  grid-column-gap: 6rem;
  grid-row-gap: 3rem;
  justify-content: center;
  align-items: center;
  padding-left: 0;
  list-style-type: none;
  display: flex;
}


.organisator-item {
  grid-column-gap: 0.5rem;
  justify-content: flex-start;
  align-items: center;
  margin-bottom: 0;
  flex-direction: row;
  display: flex;
}

.organisator_logo-wrapper {
  border: 1.5px solid var(--wp-2024--blue);
  border-radius: 50%;
  flex: none;
  width: 3rem;
  height: 3rem;
  overflow: hidden;
}
.organisator_logo {
  object-fit: cover;
  width: 100%;
  height: 100%;
}
@media screen and (max-width: 991px) {
  .organisators-list {
    flex-flow: wrap;
  }
}
@media screen and (max-width: 767px) {
  .organisators-list {
    grid-column-gap: 3rem;
  }
}
@media screen and (max-width: 479px) {
  .organisator-item {
    grid-row-gap: 1rem;
  }
  .organisators-list {
    grid-column-gap: 3rem;
    grid-row-gap: 3rem;
    grid-template-rows: auto;
    grid-template-columns: 1fr 1fr;
    grid-auto-columns: 1fr;
  }
}
</style>
