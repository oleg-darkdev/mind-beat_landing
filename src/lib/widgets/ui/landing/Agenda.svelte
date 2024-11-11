<script>
  import {agenda} from '$shared';
</script>

<section class="section_agenda">
  <div class="padding-global padding-section-medium">
    <div class="container-large">
      <a name="agenda"></a>

      <h2  class="heading">Rozkład jazdy</h2>
      <div class="spacer-xlarge"></div>
      <ul role="list" class="agenda_list">

        {#each agenda as {title, desc, time, link, linkTitle}}
        <li  class="agenda_item">
          <div class="agenda_content">
            <h3 class="text-size-large">
              {title}
            </h3>
            <p class="text-size-medium text-color-neutral">
              {desc}
            </p>
            {#if linkTitle.length > 1}
            <a href="{link}" target="_blank" class="navbar_button is-agenda w-inline-block">
              <div>{linkTitle}</div>
              <div class="button_icon w-embed">
                <svg xmlns="http://www.w3.org/2000/svg" width="100%" height="100%" viewBox="0 0 18 18" fill="none" preserveAspectRatio="xMidYMid meet" aria-hidden="true" role="img">
                  <path d="M4.38237 12.4016L10.5268 6.25717L5.7538 6.25717L5.7538 4.7574L13.0872 4.7574L13.0872 12.0908L11.5874 12.0908V7.31783L5.44303 13.4622L4.38237 12.4016Z" fill="currentColor"></path>
                </svg>
              </div>
            </a>
            {/if}

          </div>
          <div class="text-color-blue text-size-medium">{time}</div>
        </li>
        {/each}
      </ul>
    </div>
  </div>
</section>

<style>

</style>


