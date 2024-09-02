<script>
  const organisators = [
    {
      text: 'LoremIpsum',
      link: '/',
      logo: '/images/logos/darkdev_turq.svg'
    },
    {
      text: 'Serum Food&Drinks',
      link: '/',
      logo: '/images/logos/serum.png'
    },
    // {
    //   text: '',
    //   img: '',
    //   logo: ''
    // },
  ]
</script>
<!--
  <li class="orga-wp2024_item">
            <a href="{link}" target="_blank" >
            <div class="orga-wp2024_logo-wrapper">
              <img src="{logo}" loading="lazy" width="200" height="200" alt="{text} logo" class="orga-wp2024_logo">
            </div>
            <div class="text-weight-medium">{text}</div>
            </a>
          </li>
 -->
<section class="section_orga-wp2024">
    <div class="padding-section-medium">
      <div class="orga-wp2024_component">

        <a name="organisators"></a>

        <div animate="from-bottom" class="heading-wp2024">Organizatorzy</div>
        <ul role="list" class="orga-wp2024_list">
          {#each organisators as {text, link, logo}}
          <li class="orga-wp2024_item">
            <a href="{link}" target="_blank" >
            <div class="h-14">
              <img src="{logo}" loading="lazy"  alt="{text} logo" class="h-full w-full">
            </div>
            </a>
          </li>
          {/each}
            <li class="">
            <a href="/" target="_blank" class='orga-wp2024_item' >
            <div class="orga-wp2024_logo-wrapper">
              <img src="" loading="lazy" width="200" height="200" alt="" class="orga-wp2024_logo">
            </div>
            <div class="text-weight-medium">Oleg Medvedev</div>
            </a>
          </li>
        </ul>
      </div>
    </div>
  </section>
