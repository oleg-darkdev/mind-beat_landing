<script>
	// import {  } from '$lib/shared';
	import { Header, NavBar, Organisators, Agenda, Feedback, Sponsors, AboutMe, Footer, Faq} from '$lib/widgets';
  // import {  } from '$lib/entities'
</script>


<svelte:head>
  <title>MIND+BEAT</title>
</svelte:head>


<div class="page-wrapper is-wp2024">
<NavBar />

<main class="main-wrapper is-wp2024">
  <Header />

  <Organisators />

  <Agenda />

  <Sponsors />

  <div style="display:none" class="sponsor-wp2024_modal">
    <div style="opacity:0;-webkit-transform:translate3d(0, 1rem, 0) scale3d(1, 1, 1) rotateX(0) rotateY(0) rotateZ(0) skew(0, 0);-moz-transform:translate3d(0, 1rem, 0) scale3d(1, 1, 1) rotateX(0) rotateY(0) rotateZ(0) skew(0, 0);-ms-transform:translate3d(0, 1rem, 0) scale3d(1, 1, 1) rotateX(0) rotateY(0) rotateZ(0) skew(0, 0);transform:translate3d(0, 1rem, 0) scale3d(1, 1, 1) rotateX(0) rotateY(0) rotateZ(0) skew(0, 0)" class="sponsor-wp2024_modal-form-block w-form">
      <form id="wf-form-Sponsor-WWP-2024" name="wf-form-Sponsor-WWP-2024" data-name="Sponsor WWP 2024" method="get" class="sponsor-wp2024_modal-form" data-wf-page-id="66bb23c9fdc66647ff719c49" data-wf-element-id="453f0816-4073-5d61-f438-ec95e6001757">
        <div class="heading-wp2024">Sponsoriser l'événement</div>
        <div class="sponsor-wp2024_input-2col">
          <input class="sponsor-wp2024_input w-node-_06d0345e-3ea5-4af7-172d-6288220b3bb6-ff719c49 w-input" maxlength="256" name="Nom" data-name="Nom" placeholder="Nom" type="text" id="Nom" required="">
          <input class="sponsor-wp2024_input w-node-be351b65-609d-6fd7-2c85-fc13c1c571ff-ff719c49 w-input" maxlength="256" name="Prenom" data-name="Prenom" placeholder="Prénom" type="text" id="Prenom" required="">
          <input class="sponsor-wp2024_input w-node-_4bf4df32-8de9-7fd8-f194-b3c5b420402a-ff719c49 w-input" maxlength="256" name="Email" data-name="Email" placeholder="Email" type="email" id="Email" required="">
          <input class="sponsor-wp2024_input w-node-f61a0073-0982-5788-8bdf-2b9b05ef98c6-ff719c49 w-input" maxlength="256" name="Entreprise" data-name="Entreprise" placeholder="Entreprise" type="text" id="Entreprise" required="">
          <textarea placeholder="Message" maxlength="5000" id="Message" name="Message" data-name="Message" class="sponsor-wp2024_input is-text-area w-node-b2414ac2-c88f-4763-3a93-77476c512c3c-ff719c49 w-input"></textarea>
        </div>
        <button type="submit" class="button-wp2024">
          <div>Envoyer la demande de sponsor</div>
          <div class="button-wp2024_icon w-embed">
            <svg xmlns="http://www.w3.org/2000/svg" width="100%" height="100%" viewBox="0 0 18 18" fill="none" preserveAspectRatio="xMidYMid meet" aria-hidden="true" role="img">
              <path d="M4.38237 12.4016L10.5268 6.25717L5.7538 6.25717L5.7538 4.7574L13.0872 4.7574L13.0872 12.0908L11.5874 12.0908V7.31783L5.44303 13.4622L4.38237 12.4016Z" fill="currentColor"></path>
            </svg>
          </div>
        </button>
      </form>
      <div class="sponsor-wp2024_success w-form-done">
        <div class="sponsor-wp2024_modal-form">
          <div class="heading-wp2024">Nous avons bien reçu votre demande.</div>
          <div class="sponsor-wp2024_success-form">
            <p>Merci d'avoir soumis votre demande de sponsoring pour la Webflow Watch Party �&nbsp; Paris. <br>
              <br>Nous vous contacterons prochainement pour vous donner plus de détails !
            </p>
          </div>
        </div>
      </div>
      <div class="form_message-error w-form-fail">
        <div>Oups ! Un problème s'est produit lors de l'envoi du formulaire.</div>
      </div>
    </div>
    <div aria-label="fermer la modal" role="button" data-w-id="aacab12f-8def-4aa8-50c2-13e59bead31c" style="opacity:0" class="sponsor-wp2024_modal-overlay"></div>
  </div>

  <Feedback />

  <AboutMe />

  <Faq />
</main>

<Footer />
</div>


<style>

</style>
