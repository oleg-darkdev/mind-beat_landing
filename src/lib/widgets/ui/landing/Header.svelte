<script>
  import {upcomingTournaments} from '$shared';
</script>

<header class="section_header-wp2024 mb-20">
    <div class="padding-global">
      <div class="container-large">
        <div class="header-wp2024_component">
          <h1 class="heading-wp2024 is-big">Lorem Ipsum is simply</h1>

          <div class="header-wp2024_infos-wrapper">
            {#each upcomingTournaments as {place, date, time}}
            <div  class="header-wp2024_item">
              <div class="wp2024-tag">{place}</div>
              <div class="text-size-large">{date}</div>
              <div class="text-size-medium text-color-neutral-wp2024">Start {time}</div>
            </div>
            {/each}
          </div>

          <div class="header-wp2024_description-wrapper">
            <p class="text-size-medium">
              Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
            </p>

            <a href="/" class="button-wp2024 w-inline-block">
              <div>Lorem Ipsum has been</div>
              <div class="button-wp2024_icon w-embed">
                <svg xmlns="http://www.w3.org/2000/svg" width="100%" height="100%" viewBox="0 0 18 18" fill="none" preserveAspectRatio="xMidYMid meet" aria-hidden="true" role="img">
                  <path d="M4.38237 12.4016L10.5268 6.25717L5.7538 6.25717L5.7538 4.7574L13.0872 4.7574L13.0872 12.0908L11.5874 12.0908V7.31783L5.44303 13.4622L4.38237 12.4016Z" fill="currentColor"></path>
                </svg>
              </div>
            </a>

          </div>
          <div class="date-countdown heading-wp2024 is-big">2024</div>
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
