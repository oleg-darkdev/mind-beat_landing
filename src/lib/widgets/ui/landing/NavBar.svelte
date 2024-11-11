<script>
  import {navigation, RegistrationBtn, GoSponsor} from '$shared';

  let showMenu = false;
</script>

<div class="navbar_component w-nav py-2" role="banner">
  <nav role="navigation" class="navbar_menu {showMenu ? 'h-[22rem]': ''} w-nav-menu desctop-hidden">

    <div class="relative">
      <div class="grid grid-cols-2 gap-4">
      <GoSponsor />

      <RegistrationBtn />
    </div>
  </div>

    {#if showMenu}
      <div class='flex flex-col'>
        {#each navigation as {title, link}}
          <a href="{link}" class="navbar_link w-nav-link">{title}</a>
        {/each}
      </div>
    {/if}
  </nav>


  <div class="navbar_container ">
    <div class="navbar_menu-button w-nav-button flex flex-row justify-between w-full desctop-hidden">
      <div class="h-10 w-auto">
        <img src="/images/logo.svg" alt="MIND+BEAT logo">
      </div>

      <div class="menu-icon3" on:click={()=> showMenu = !showMenu}>
        <div class="menu-icon3_line-top"></div>
        <div class="menu-icon3_line-middle"></div>
        <div class="menu-icon3_line-bottom"></div>
      </div>
    </div>



    <nav role="navigation" class=" navbar_menu w-nav-menu flex flex-row  mobile-hidden">
      <div class=" h-10 w-40">
        <img src="/images/logo.svg" alt="MIND+BEAT logo">
      </div>

      <div class='mr-20'>
        {#each navigation as {title, link}}
          <a href="{link}" class="navbar_link w-nav-link">{title}</a>
        {/each}
      </div>

      <div class="grid grid-cols-2 ">
        <GoSponsor />

        <RegistrationBtn />
      </div>
    </nav>
  </div>
</div>


<style>
@media screen and (max-width: 991px) {
  .mobile-hidden {
    display: none;
  }
  .navbar_menu-button {
    z-index: 3;
    margin-left: -0.5rem;
    padding: 0;
    background-color: #0000;
  }
    .navbar_container {
    z-index: 2;
    flex-flow: row-reverse;
    grid-auto-columns: 1fr;
  }
  .navbar_menu {
    z-index: 2;
    background-color: var(--wp-2024--neutral-dark);
    flex-flow: column;
    width: 100%;
    margin-left: 0;
    padding: 2rem 2.5rem 5rem;
    font-size: 1.125rem;
    transition: height 0.5s;
    position: absolute;
    inset: 4.5rem 0 0% auto;
    overflow: hidden;
  }
}
@media screen and (max-width: 767px) {
  .navbar_menu {
    /* height: 16rem; */
    padding-top: 1rem;
    padding-left: 1.25rem;
    padding-right: 1.25rem;
  }
}

@media screen and (min-width: 991px) {
  .desctop-hidden {
    display: none;
  }
}



.navbar_menu-button {
  padding: 0;
}
.navbar_container {
  grid-column-gap: 1rem;
  grid-row-gap: 1rem;
  grid-template-rows: auto;
  grid-template-columns: 1fr max-content 1fr;
  grid-auto-columns: 1fr;
  justify-content: space-between;
  place-items: center stretch;
  width: 100%;
  max-width: 80rem;
  height: 100%;
  margin-left: auto;
  margin-right: auto;
  display: flex;
}
.w-nav-button {
  float: right;
  cursor: pointer;
  -webkit-tap-highlight-color: #0000;
  tap-highlight-color: #0000;
  -webkit-user-select: none;
  user-select: none;
  padding: 18px;
  font-size: 24px;
  /* display: none; */
  position: relative;
}
.w-nav-button:focus {
  outline: 0;
}
.w-nav-button.w--open {
  color: #fff;
  background-color: #c8c8c8;
}

</style>
