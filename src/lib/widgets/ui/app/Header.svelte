<script>
  import {upcomingTournaments, RegistrationBtn} from '$shared';
</script>

<header class="section_header-wp2024 mb-20">
    <div class="padding-global">
      <div class="container-large">
        <div class="header-wp2024_component">
          <h1 class="heading-wp2024 is-big">
            Gra umysłu i rytm serca.
          </h1>

          <div class="header-wp2024_infos-wrapper">
            <!-- {#each upcomingTournaments.slice(0,3) as {place, date, time, location}}
            <div  class="header-wp2024_item">
              <a href="{location}" target='_blank '>
                <div class="wp2024-tag">{place}</div>
              </a>
              <div class="text-size-large">{date}</div>
              <div class="text-size-medium text-color-neutral-wp2024">Start {time}</div>
            </div>
            {/each} -->
          </div>

          <div class="header-wp2024_description-wrapper">
            <p class="text-size-medium text-size-medium navbar-wp2024_button is-programme w-inline-block">
              1. Podejdź do <a href="https://mind-beat.vercel.app/#contact" class='wp2024-tag' target="_blank" >sędziego
                </a>   i zarejestruj się w turnieju.
            </p>
            <p class="text-size-medium text-size-medium navbar-wp2024_button is-programme w-inline-block">
              2. Zapoznaj się z <a href="https://mind-beat.vercel.app/#agenda" class='wp2024-tag' target="_blank" >harmonogramem turnieju
                </a> i trzymaj się go.
            </p>
            <p class="text-size-medium navbar-wp2024_button is-programme w-inline-block">
              3. Kliknij <a href="https://ralfs-gutmanis.github.io/novuss-clock/" class='wp2024-tag' target="_blank">link do elektronicznego zegara szachowego  </a>  i ustaw 600 sekund w ustawieniach.
            </p>
            <p class="text-size-medium text-size-medium navbar-wp2024_button is-programme w-inline-block">
              4. Po zakończeniu gry - zgłoś wynik sędziemu.
            </p>

            <!-- <RegistrationBtn /> -->

          </div>

          <!-- <div class='flex justify-end items-end content-end flex-col'>
            <span class="date-countdown heading-wp2024 text-size-large">
              Harmonogram na rok
            </span>
            <div class="date-countdown heading-wp2024 is-big">2024</div>
          </div> -->

        </div>
      </div>
    </div>
    <img src="images/bg-1.jpg" loading="lazy" alt="" class="header-wp2024_decoration">
  </header>

<style>
.section_header-wp2024 {
  z-index: 1;
  position: relative;
}
.button-wp2024_icon {
  /* z-index: 1;
  justify-content: center;
  align-items: center; */
  width: 1.125rem;
  height: 1.125rem;
  /* transition: right 0.2s, top 0.2s; */
  /* display: flex;
  position: relative; */
  /* inset: 0 0 auto auto; */
}
.header-wp2024_item {
  grid-row-gap: 0.5rem;
  flex-flow: column;
  justify-content: flex-start;
  align-items: flex-end;
  display: flex;
}
.header-wp2024_infos-wrapper {
  grid-row-gap: 2rem;
  flex-flow: column;
  flex: none;
  display: flex;
}

.header-wp2024_component {
  grid-column-gap: 2rem;
  grid-row-gap: 2rem;
  flex-flow: column;
  grid-template-rows: auto;
  grid-template-columns: 1fr 0.55fr;
  grid-auto-columns: 1fr;
  justify-content: space-between;
  align-items: stretch;
  height: calc(100vh - 4.5rem);
  padding-top: 3rem;
  padding-bottom: 3rem;
  display: grid;
}
.date-countdown {
  place-self: end;
}

@media screen and (max-width: 991px) {
  .header-wp2024_item {
    justify-content: flex-start;
    align-items: flex-start;
  }
  .header-wp2024_infos-wrapper {
    grid-column-gap: 2rem;
    grid-row-gap: 2rem;
    flex-flow: row;
    grid-template-rows: auto;
    grid-template-columns: 1fr 1fr 1fr;
    grid-auto-columns: 1fr;
    width: 100%;
    margin-top: 2rem;
    display: grid;
  }
  .header-wp2024_component {
    grid-row-gap: 0rem;
    grid-template-columns: 1fr;
    height: auto;
  }
  .date-countdown {
    grid-area: 2/1/3/2;
    justify-self: start;
  }
}

@media screen and (max-width: 767px) {
  .header-wp2024_infos-wrapper {
    grid-template-columns: 1fr;
  }
  .header-wp2024_component {
    padding-top: 2rem;
    padding-bottom: 2rem;
  }
}
</style>
