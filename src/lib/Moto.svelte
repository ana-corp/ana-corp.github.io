<script>
  import { motoPerusahaan, namaPerusahaan } from "./data";
</script>

<section id="quote" class="parallax-section-6">
  <div class="container">
    <div class="row wow fadeInUp">
      <div class="col-lg-12 wow fadeInUp" style="z-index:3">
        <div id="quote-slider">
          <div id="moto">
            <blockquote>
              <span class="icon">
                <svg
                  class="inverse"
                  width="1.5em"
                  height="1.5em"
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 24 24"
                  fill="currentColor"
                  ><path d="M0 0h24v24H0z" fill="none"></path><path
                    d="M6 17h3l2-4V7H5v6h3zm8 0h3l2-4V7h-6v6h3z"
                  ></path></svg
                >
              </span>
              <span>{motoPerusahaan}</span>
              <span class="icon">
                <svg
                  width="1.5em"
                  height="1.5em"
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 24 24"
                  fill="currentColor"
                  ><path d="M0 0h24v24H0z" fill="none"></path><path
                    d="M6 17h3l2-4V7H5v6h3zm8 0h3l2-4V7h-6v6h3z"
                  ></path></svg
                >
              </span>
            </blockquote>
            <strong style="text-align:center; display:block;">
              <em class="highlight">
                {namaPerusahaan || "Company"}
              </em>
            </strong>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<style>
  svg {
    vertical-align: middle;
    fill: #91da32;
    transform: translateY(-20%);
    display: inline-block;
  }

  .inverse {
    transform: rotateY(180deg) translateY(-20%);
  }

  #quote blockquote span {
    padding: 0;
  }
</style>
