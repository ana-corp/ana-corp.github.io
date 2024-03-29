<script>
  import List from "./List.svelte";
  import { misi, sejarahPerusahaan, visi } from "./data";
</script>

<section id="about" class="parallax-section-1">
  <div class="container">
    <div class="text-center col-md-12 wow fadeInUp">
      <h3 class="section-title">Tentang Perusahaan.</h3>
      <p class="subheading" id="overview"></p>
    </div>

    <!-- VISI -->
    <div>
      <h3 class="text-center wow fadeInUp visi">VISI</h3>
      <div class="row features-row wow fadeInUp" id="visiList">
        <List data={visi} />
      </div>
    </div>

    <!-- MISI -->
    <div>
      <h3 class="text-center wow fadeInUp visi">MISI</h3>
      <div class="row features-row wow fadeInUp" id="misiList">
        <List data={misi} />
      </div>
    </div>
  </div>

  <section>
    <div class="container">
      <div class="row">
        <div class="text-left about-text" style="padding: 4rem;">
          <h3 class="wow fadeInUp">Histori</h3>
          {#each sejarahPerusahaan as p}
            <p class="wow fadeInUp">
              {@html p}
            </p>
          {/each}
          <p class="wow fadeInUp">
            <a href="#contact" class="btn btn-primary btn-md">Hubungi Kami</a>
          </p>
        </div>
      </div>
    </div>
  </section>
</section>
