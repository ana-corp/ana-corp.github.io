<script>
  import About from "$lib/About.svelte";
  import Contact from "$lib/Contact.svelte";
  import Header from "$lib/Header.svelte";
  import Moto from "$lib/Moto.svelte";
  import Point from "$lib/Point.svelte";
  import Product from "$lib/Product.svelte";
  import Slider from "$lib/Slider.svelte";
  import Struktur from "$lib/Struktur.svelte";
  import { motoPerusahaan, namaPerusahaan } from "$lib/data";
</script>

<svelte:head>
  <link
    rel="stylesheet"
    href="/bootstrap/css/bootstrap.min.css"
    type="text/css"
  />
  <link
    rel="stylesheet"
    href="/css/font-awesome/css/font-awesome.css"
    type="text/css"
  />
  <link rel="stylesheet" href="/css/style.css" type="text/css" />

  <link rel="stylesheet" href="/css/colors/green.css" id="color-skins" />

  <script type="text/javascript" defer src="/js/plugins/jquery.min.js"></script>
  <script
    type="text/javascript"
    defer
    src="/bootstrap/js/bootstrap.min.js"
  ></script>
  <script type="text/javascript" defer src="/js/scripts.js"></script>
</svelte:head>
<Header />
<Slider />
<div class="site-wrapper content">
  <About />
  <Product />
  <Struktur />
  <Moto />
  <Point />
  <Contact />
  <a id="back-to-top" href={"#"}>
    <svg
      width="24"
      height="24"
      xmlns="http://www.w3.org/2000/svg"
      fill="none"
      viewBox="0 0 24 24"
      stroke="currentColor"
      ><path
        stroke-linecap="round"
        stroke-linejoin="round"
        stroke-width="2"
        d="M5 15l7-7 7 7"
      ></path></svg
    >
  </a>
</div>

<style>
  :global(html) {
    scroll-behavior: smooth;
  }

  SVG {
    vertical-align: middle;
  }

  #back-to-top {
    position: fixed;
    bottom: 3.5rem;
    right: 3.5rem;
    transform: translateY(10vh);
    opacity: 0;
    will-change: transform;
    transition:
      transform 300ms cubic-bezier(0.645, 0.045, 0.355, 1),
      opacity 350ms cubic-bezier(0.19, 1, 0.22, 1);
  }

  :global(#back-to-top.active) {
    transform: translateY(0);
    opacity: 1;
  }
</style>
