---
layout: null
permalink: /GS_Trans_UNet/
---
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <meta name="description"
        content="GS-TransUNet: integrated 2D Gaussian splatting and transformer UNet for accurate skin lesion analysis">
  <meta name="keywords" content="Image Diffusion, Data Attribution, Style Attribution, Stable Diffusion">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>GS-TransUNet: Integrated 2D Gaussian splatting and transformer UNet for accurate skin lesion analysis</title>

  <!-- Global site tag (gtag.js) - Google Analytics -->
  <!-- <script async src="https://www.googletagmanager.com/gtag/js?id=G-PYVRSFMDRL"></script>
  <script>
    window.dataLayer = window.dataLayer || [];

    function gtag() {
      dataLayer.push(arguments);
    }

    gtag('js', new Date());

    gtag('config', 'G-PYVRSFMDRL');
  </script> -->

  <link href="https://fonts.googleapis.com/css?family=Google+Sans|Noto+Sans|Castoro"
        rel="stylesheet">

  <link rel="stylesheet" href="{{ '/assets/html/GS_Trans_UNet/static/css/bulma.min.css' | relative_url }}">
  <link rel="stylesheet" href="{{ '/assets/html/GS_Trans_UNet/static/css/bulma-carousel.min.css' | relative_url }}">
  <link rel="stylesheet" href="{{ '/assets/html/GS_Trans_UNet/static/css/bulma-slider.min.css' | relative_url }}">
  <link rel="stylesheet" href="{{ '/assets/html/GS_Trans_UNet/static/css/fontawesome.all.min.css' | relative_url }}">
  <link rel="stylesheet"
        href="https://cdn.jsdelivr.net/gh/jpswalsh/academicons@1/css/academicons.min.css">
  <link rel="stylesheet" href="{{ '/assets/html/GS_Trans_UNet/static/css/index.css' | relative_url }}">
  <link rel="icon" href="{{ '/assets/html/GS_Trans_UNet/static/images/favicon.png' | relative_url }}">

  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
  <script defer src="{{ '/assets/html/GS_Trans_UNet/static/js/fontawesome.all.min.js' | relative_url }}"></script>
  <script src="{{ '/assets/html/GS_Trans_UNet/static/js/bulma-carousel.min.js' | relative_url }}"></script>
  <script src="{{ '/assets/html/GS_Trans_UNet/static/js/bulma-slider.min.js' | relative_url }}"></script>
  <script src="{{ '/assets/html/GS_Trans_UNet/static/js/index.js' | relative_url }}"></script>
</head>
<body>

<nav class="navbar" role="navigation" aria-label="main navigation">
  <div class="navbar-brand">
    <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false">
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </a>
  </div>
  <div class="navbar-menu">
    <div class="navbar-start" style="flex-grow: 1; justify-content: center;">
      <a class="navbar-item" href="https://anandk27.github.io/">
      <span class="icon">
          <i class="fas fa-home"></i>
      </span>
      </a>

      <!-- <div class="navbar-item has-dropdown is-hoverable">
        <a class="navbar-link">
          More Research
        </a>
        <div class="navbar-dropdown">
          <a class="navbar-item" href="https://hypernerf.github.io">
            HyperNeRF
          </a>
          <a class="navbar-item" href="https://nerfies.github.io">
            Nerfies
          </a>
          <a class="navbar-item" href="https://latentfusion.github.io">
            LatentFusion
          </a>
          <a class="navbar-item" href="https://photoshape.github.io">
            PhotoShape
          </a>
        </div>
      </div> -->
    </div>

  </div>
</nav>


<section class="hero">
  <div class="hero-body">
    <div class="container is-max-desktop">
      <div class="columns is-centered">
        <div class="column has-text-centered">
          <h1 class="title is-1 publication-title">GS-TransUNet</h1>
            <h2 class="title is-2 publication-title">Integrated 2D Gaussian splatting and transformer UNet for accurate skin lesion analysis</h2>
          <h3 class="title is-size-3 publication-venue">SPIE Medical Imaging 2025</h3>
          <div class="is-size-5 publication-authors">
            <span class="author-block">
              <a href="https://anandk27.github.io/">Anand Kumar</a><sup>1</sup>,</span>
            <span class="author-block">
              <a href="https://www.linkedin.com/in/kavinder-roghit/">Kavinder Roghit</a><sup>1</sup>,</span>
            <span class="author-block">
              <a href="https://www.linkedin.com/in/josnajohn/">Josna John</a><sup>1</sup>,
            </span>
          </div>

          <div class="is-size-5 publication-authors">
            <span class="author-block"><sup>1</sup>University of California, San Diego</span>
          </div>

          <div class="column has-text-centered">
            <div class="publication-links">
              <!-- PDF Link. -->
              <!-- <span class="link-block">
                <a href="{{ '/assets/html/GS_Trans_UNet/static/paper.pdf' | relative_url }}"
                   class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                      <i class="fas fa-file-pdf"></i>
                  </span>
                  <span>Paper</span>
                </a>
              </span> -->
                            <span class="link-block">
                <a href="https://www.spiedigitallibrary.org/conference-proceedings-of-spie/13407/1340736/GS-TransUNet--integrated-2D-Gaussian-splatting-and-transformer-UNet/10.1117/12.3046869.short"
                   class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                      <i class="fas fa-book-open"></i>
                  </span>
                  <span>SPIE</span>
                </a>
              </span>
              <span class="link-block">
                <a href="https://arxiv.org/abs/2502.16748"
                   class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                      <i class="ai ai-arxiv"></i>
                  </span>
                  <span>arXiv</span>
                </a>
              </span>
              <!-- Video Link. -->
              <!-- <span class="link-block">
                <a href="https://www.youtube.com/watch?v=MrKrnHhk8IA"
                   class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                      <i class="fab fa-youtube"></i>
                  </span>
                  <span>Video</span>
                </a>
              </span> -->
              <!-- Code Link. -->
              <span class="link-block">
                <a href="https://github.com/AnandK27/GS-TransUNet"
                   class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                      <i class="fab fa-github"></i>
                  </span>
                  <span>Code</span>
                  </a>
              </span>
              <!-- Dataset Link. -->
              <!-- <span class="link-block">
                <a href="https://github.com/google/nerfies/releases/tag/0.1"
                   class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                      <i class="far fa-images"></i>
                  </span>
                  <span>Data</span>
                  </a>
                </span> -->
            </div>

          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="hero teaser">
  <div class="container is-max-desktop">
    <div class="hero-body">
      <!-- <video id="teaser" autoplay muted loop playsinline height="100%">
        <source src="./static/videos/teaser.mp4"
                type="video/mp4">
      </video> -->
      <embed src="{{ '/assets/html/GS_Trans_UNet/static/images/poster.pdf' | relative_url }}" width="100%" height="600px" type="application/pdf" id="teaser" style="border:none;">
      <p><a href="{{ '/assets/html/GS_Trans_UNet/static/images/poster.pdf' | relative_url }}">Download the Poster</a>.</p>

    </div>
  </div>
</section>


<!-- <section class="hero is-light is-small">
  <div class="hero-body">
    <div class="container is-max-desktop has-text-centered">
      <h3 class="title has-text-centered is-3">Retrieval Results</h3>
      <div id="results-carousel" class="carousel results-carousel">
        <div class="item item-1">
          <img src="./static/images/car_1.png" id="item-1"
               class="interpolation-image"/>
        </div>
        <div class="item item-1">
          <img src="./static/images/car_2.png" id="item-1"
                class="interpolation-image"/>
        </div>
        <div class="item item-1">
          <img src="./static/images/car_3.png" id="item-1"
               class="interpolation-image"/>
        </div>
        <div class="item item-1">
          <img src="./static/images/car_4.png" id="item-1"
               class="interpolation-image"/>
        </div>
        <div class="item item-1">
          <img src="./static/images/car_5.png" id="item-1"
               class="interpolation-image"/>
        </div>
        
      </div>
      <div class="content has-text-centered">
        The first left column is the query image with remaining columns showing retreival results with <span style="color: green;">green</span> colors for correct and <span style="color: rgba(222, 72, 72, 0.84);">red</span> for incorrect retrievals.
      </div>
    </div>
  </div>
</section> -->


<section class="section">
  <div class="container is-max-desktop">
    <!-- Abstract. -->
    <div class="columns is-centered has-text-centered">
      <div class="column is-four-fifths">
        <h2 class="title is-3">Abstract</h2>
        <div class="content has-text-justified">
          <!-- <p>
            We present the first method capable of photorealistically reconstructing a non-rigidly
            deforming scene using photos/videos captured casually from mobile phones.
          </p> -->
          <p>
          We can achieve fast and consistent early skin cancer detection with recent developments in computer vision and deep learning techniques. However, the existing skin lesion segmentation and classification prediction models run independently, thus missing potential efficiencies from their integrated execution.
          </p>
          <p>
          To unify skin lesion analysis, our paper presents the <b>Gaussian Splatting - Transformer UNet (GS-TransUNet)</b>, a novel approach that synergistically combines 2D Gaussian splatting with the Transformer UNet architecture for automated skin cancer diagnosis. Our unified deep learning model efficiently delivers dual-function skin lesion classification and segmentation for clinical diagnosis. Evaluated on ISIC-2017 and PH2 datasets, our network demonstrates superior performance compared to existing state-of-the-art models across multiple metrics through 5-fold cross-validation. Our findings illustrate significant advancements in the precision of segmentation and classification. This integration sets new benchmarks in the field and highlights the potential for further research into multi-task medical image analysis methodologies, promising enhancements in automated diagnostic systems.</p>
          <!-- <p>
            We show that <span class="dnerf">Nerfies</span> can turn casually captured selfie
            photos/videos into deformable NeRF
            models that allow for photorealistic renderings of the subject from arbitrary
            viewpoints, which we dub <i>"nerfies"</i>. We evaluate our method by collecting data
            using a
            rig with two mobile phones that take time-synchronized photos, yielding train/validation
            images of the same pose at different viewpoints. We show that our method faithfully
            reconstructs non-rigidly deforming scenes and reproduces unseen views with high
            fidelity.
          </p> -->
        </div>
      </div>
    </div>
    </div>
</section>
    <!--/ Abstract. -->





<section class="section">
  <div class="container is-max-desktop">
    
    <!--/ Paper video. -->

    <!-- <div class="columns is-centered"> -->

      <!-- Visual Effects. -->
      <!-- <div class="column">
        <div class="content">
          <h2 class="title is-3">Visual Effects</h2>
          <p>
            Using <i>nerfies</i> you can create fun visual effects. This Dolly zoom effect
            would be impossible without nerfies since it would require going through a wall.
          </p>
          <video id="dollyzoom" autoplay controls muted loop playsinline height="100%">
            <source src="./static/videos/dollyzoom-stacked.mp4"
                    type="video/mp4">
          </video>
        </div>
      </div> -->
      <!--/ Visual Effects. -->

      <!-- Matting. -->
      <!-- <div class="column">
        <h2 class="title is-3">Matting</h2>
        <div class="columns is-centered">
          <div class="column content">
            <p>
              As a byproduct of our method, we can also solve the matting problem by ignoring
              samples that fall outside of a bounding box during rendering.
            </p>
            <video id="matting-video" controls playsinline height="100%">
              <source src="./static/videos/matting.mp4"
                      type="video/mp4">
            </video>
          </div>

        </div>
      </div>
    </div> -->
    <!--/ Matting. -->

    <!-- Animation. -->
    <!-- <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Animation</h2> -->

        <!-- Interpolating. -->
        <!-- <h3 class="title is-4">Interpolating states</h3>
        <div class="content has-text-justified">
          <p>
            We can also animate the scene by interpolating the deformation latent codes of two input
            frames. Use the slider here to linearly interpolate between the left frame and the right
            frame.
          </p>
        </div>
        <div class="columns is-vcentered interpolation-panel">
          <div class="column is-3 has-text-centered">
            <img src="./static/images/interpolate_start.jpg"
                 class="interpolation-image"
                 alt="Interpolate start reference image."/>
            <p>Start Frame</p>
          </div>
          <div class="column interpolation-video-column">
            <div id="interpolation-image-wrapper">
              Loading...
            </div>
            <input class="slider is-fullwidth is-large is-info"
                   id="interpolation-slider"
                   step="1" min="0" max="100" value="0" type="range">
          </div>
          <div class="column is-3 has-text-centered">
            <img src="./static/images/interpolate_end.jpg"
                 class="interpolation-image"
                 alt="Interpolation end reference image."/>
            <p class="is-bold">End Frame</p>
          </div>
        </div>
        <br/> -->
        <!--/ Interpolating. -->

        <!-- Re-rendering. -->
        <!-- <h3 class="title is-4">Re-rendering the input video</h3>
        <div class="content has-text-justified">
          <p>
            Using <span class="dnerf">Nerfies</span>, you can re-render a video from a novel
            viewpoint such as a stabilized camera by playing back the training deformations.
          </p>
        </div>
        <div class="content has-text-centered">
          <video id="replay-video"
                 controls
                 muted
                 preload
                 playsinline
                 width="75%">
            <source src="./static/videos/replay.mp4"
                    type="video/mp4">
          </video>
        </div> -->
        <!--/ Re-rendering. -->
<!-- 
      </div>
    </div> -->
    <!--/ Animation. -->


    <!-- Concurrent Work. -->
    <!-- <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Related Links</h2>

        <div class="content has-text-justified">
          <p>
            There's a lot of excellent work that was introduced around the same time as ours.
          </p>
          <p>
            <a href="https://arxiv.org/abs/2104.09125">Progressive Encoding for Neural Optimization</a> introduces an idea similar to our windowed position encoding for coarse-to-fine optimization.
          </p>
          <p>
            <a href="https://www.albertpumarola.com/research/D-NeRF/index.html">D-NeRF</a> and <a href="https://gvv.mpi-inf.mpg.de/projects/nonrigid_nerf/">NR-NeRF</a>
            both use deformation fields to model non-rigid scenes.
          </p>
          <p>
            Some works model videos with a NeRF by directly modulating the density, such as <a href="https://video-nerf.github.io/">Video-NeRF</a>, <a href="https://www.cs.cornell.edu/~zl548/NSFF/">NSFF</a>, and <a href="https://neural-3d-video.github.io/">DyNeRF</a>
          </p>
          <p>
            There are probably many more by the time you are reading this. Check out <a href="https://dellaert.github.io/NeRF/">Frank Dellart's survey on recent NeRF papers</a>, and <a href="https://github.com/yenchenlin/awesome-NeRF">Yen-Chen Lin's curated list of NeRF papers</a>.
          </p>
        </div>
      </div>
    </div> -->
    <!--/ Concurrent Work. -->

  </div>
</section>


<section class="section" id="BibTeX">
  <div class="container is-max-desktop content">
    <h2 class="title">BibTeX</h2>
    <pre><code>@inproceedings{kumar2024gstransunet,
  author = {Kumar, Anand and Kavinder Roghit, Kanthen and John, Josna},
  booktitle = {Medical Imaging 2025: AI/ML},
  organization = {SPIE},
  title = {GS-TransUNet: integrated 2D Gaussian splatting and transformer UNet for accurate skin lesion analysis},
  month = nov,
  year = {2024},
  doi = {10.1117/12.3046869}
}</code></pre>
  </div>
</section>


<footer class="footer">
  <div class="container">
    <div class="content has-text-centered">
      <!-- <a class="icon-link"
         href="./static/videos/nerfies_paper.pdf">
        <i class="fas fa-file-pdf"></i>
      </a> -->
      <a class="icon-link" href="https://github.com/AnandK27" class="external-link" disabled>
        <i class="fab fa-github"></i>
      </a>
    </div>
    <div class="columns is-centered">
      <div class="column is-8">
        <div class="content">
          <p>
            Template has been borrowed from <a
              href="https://github.com/nerfies/nerfies.github.io">Nerfies</a>.
          </p>
        </div>
      </div>
    </div>
  </div>
</footer>

</body>
</html>
