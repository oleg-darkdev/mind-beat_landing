<script>
	// import {  } from '$lib/shared';
	import { Header, NavBar, Organisators, Awards, Agenda, Feedback, Sponsors, AboutMe, Footer, Faq} from '$lib/widgets';
  // import {  } from '$lib/entities'
</script>


<svelte:head>
  <title>MIND+BEAT</title>
</svelte:head>


<div class="page-wrapper is">
<NavBar />

<main class="main-wrapper is">
  <Header />

  <Organisators />

  <Agenda />

  <Awards />

  <Sponsors />

  <Feedback />

  <Faq />

  <AboutMe />
</main>

<Footer />
</div>


<style>

</style>
