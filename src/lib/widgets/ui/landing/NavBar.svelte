<script>
  const navigation = [
    // {
    //   title: '',
    //   link: '#'
    // },
    {
      title: 'Organizatorzy',
      link: '#organisators'
    },

    {
      title: 'Rozkład jazdy',
      link: '#agenda'
    },
    {
      title: 'Sponsorzy',
      link: '#sponsors'
    },
    {
      title: 'Opinie',
      link: '#report'
    },
    {
      title: 'Contact',
      link: '#contact'
    },
  ]
</script>

<div  class="navbar-wp2024_component w-nav" role="banner">
  <div class="navbar-wp2024_container">
    <div class="navbar-wp2024_menu-button w-nav-button">
      <div class="menu-icon3">
        <div class="menu-icon3_line-top"></div>
        <div class="menu-icon3_line-middle"></div>
        <div class="menu-icon3_line-bottom"></div>
      </div>
    </div>
    <nav role="navigation" class="navbar-wp2024_menu w-nav-menu">
      <div class="h-10 w-40">
        <img src="/images/logo.svg" alt="MIND+BEAT logo">
      </div>
      {#each navigation as {title, link}}
        <a href="{link}" class="navbar-wp2024_link w-nav-link">{title}</a>
      {/each}

      <a href="" target="_blank" class="navbar-wp2024_button w-inline-block">
        <div>Lorem imposum</div>
        <div class="button-wp2024_icon w-embed">
          <svg xmlns="http://www.w3.org/2000/svg" width="100%" height="100%" viewBox="0 0 18 18" fill="none" preserveAspectRatio="xMidYMid meet" aria-hidden="true" role="img">
            <path d="M4.38237 12.4016L10.5268 6.25717L5.7538 6.25717L5.7538 4.7574L13.0872 4.7574L13.0872 12.0908L11.5874 12.0908V7.31783L5.44303 13.4622L4.38237 12.4016Z" fill="currentColor"></path>
          </svg>
        </div>
      </a>
    </nav>

    <a href="" class="button-wp2024 w-inline-block">
      <div>Lorem imposum</div>
      <div class="button-wp2024_icon w-embed">
        <svg xmlns="http://www.w3.org/2000/svg" width="100%" height="100%" viewBox="0 0 18 18" fill="none" preserveAspectRatio="xMidYMid meet" aria-hidden="true" role="img">
          <path d="M4.38237 12.4016L10.5268 6.25717L5.7538 6.25717L5.7538 4.7574L13.0872 4.7574L13.0872 12.0908L11.5874 12.0908V7.31783L5.44303 13.4622L4.38237 12.4016Z" fill="currentColor"></path>
        </svg>
      </div>
    </a>
  </div>
</div>


<style>

</style>
