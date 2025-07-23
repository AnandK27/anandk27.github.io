---
layout: null
permalink: /IntroStyle/
---
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <meta name="description"
        content="IntroStyle: Training-Free Introspective Style Attribution using Diffusion Features">
  <meta name="keywords" content="Image Diffusion, Data Attribution, Style Attribution, Stable Diffusion">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>IntroStyle: Training-Free Introspective Style Attribution using Diffusion Features</title>

  <link href="https://fonts.googleapis.com/css?family=Google+Sans|Noto+Sans|Castoro"
        rel="stylesheet">

  <link rel="stylesheet" href="{{ '/assets/html/IntroStyle/static/css/bulma.min.css' | relative_url }}">
  <link rel="stylesheet" href="{{ '/assets/html/IntroStyle/static/css/bulma-carousel.min.css' | relative_url }}">
  <link rel="stylesheet" href="{{ '/assets/html/IntroStyle/static/css/bulma-slider.min.css' | relative_url }}">
  <link rel="stylesheet" href="{{ '/assets/html/IntroStyle/static/css/fontawesome.all.min.css' | relative_url }}">
  <link rel="stylesheet"
        href="https://cdn.jsdelivr.net/gh/jpswalsh/academicons@1/css/academicons.min.css">
  <link rel="stylesheet" href="{{ '/assets/html/IntroStyle/static/css/index.css' | relative_url }}">
  <link rel="icon" href="{{ '/assets/html/IntroStyle/static/images/favicon.png' | relative_url }}">

  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
  <script defer src="{{ '/assets/html/IntroStyle/static/js/fontawesome.all.min.js' | relative_url }}"></script>
  <script src="{{ '/assets/html/IntroStyle/static/js/bulma-carousel.min.js' | relative_url }}"></script>
  <script src="{{ '/assets/html/IntroStyle/static/js/bulma-slider.min.js' | relative_url }}"></script>
  <script src="{{ '/assets/html/IntroStyle/static/js/index.js' | relative_url }}"></script>
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
    </div>
  </div>
</nav>

<section class="hero">
  <div class="hero-body">
    <div class="container is-max-desktop">
      <div class="columns is-centered">
        <div class="column has-text-centered">
          <h1 class="title is-1 publication-title">IntroStyle: Training-Free Introspective Style Attribution using Diffusion Features</h1>
          <h3 class="title is-size-3 publication-venue">ICCV 2025</h3>
          <div class="is-size-5 publication-authors">
            <span class="author-block">
              <a href="https://anandk27.github.io/">Anand Kumar</a><sup>1</sup>,</span>
            <span class="author-block">
              <a href="https://jitengmu.github.io/">Jiteng Mu</a><sup>1</sup>,</span>
            <span class="author-block">
              <a href="http://www.svcl.ucsd.edu/people/nuno/">Nuno Vasconcelos</a><sup>1</sup>,
            </span>
          </div>

          <div class="is-size-5 publication-authors">
            <span class="author-block"><sup>1</sup>University of California, San Diego</span>
          </div>

          <div class="column has-text-centered">
            <div class="publication-links">
              <span class="link-block">
                <a href="{{ '/assets/html/IntroStyle/static/paper.pdf' | relative_url }}"
                   class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                      <i class="fas fa-file-pdf"></i>
                  </span>
                  <span>Paper</span>
                </a>
              </span>
              <span class="link-block">
                <a href="https://arxiv.org/abs/2412.14432"
                   class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                      <i class="ai ai-arxiv"></i>
                  </span>
                  <span>arXiv</span>
                </a>
              </span>
              <span class="link-block">
                <a href="https://github.com/AnandK27/IntroStyle"
                   class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                      <i class="fab fa-github"></i>
                  </span>
                  <span>Code</span>
                  </a>
              </span>
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
      <img src="{{ '/assets/html/IntroStyle/static/images/teaser.png' | relative_url }}" alt="IntroStyle teaser image." id="teaser" height="100%"/>
      <h2 class="subtitle has-text-centered">
        <span class="texttt">IntroStyle</span> a metric for style measurement.
        Top two rows are retreival results with <span style="color: green;">green</span> colors for correct and <span style="color: rgba(222, 72, 72, 0.84);">red</span> for incorrect retrievals.
        The bottom row shows ranking with lower score for images further away in style from the reference in the first column. 
      </h2>
    </div>
  </div>
</section>

<section class="hero is-light is-small">
  <div class="hero-body">
    <div class="container is-max-desktop has-text-centered">
      <h3 class="title has-text-centered is-3">Retrieval Results</h3>
      <div id="results-carousel" class="carousel results-carousel">
        <div class="item item-1">
          <img src="{{ '/assets/html/IntroStyle/static/images/car_1.png' | relative_url }}" id="item-1"
               class="interpolation-image"/>
        </div>
        <div class="item item-1">
          <img src="{{ '/assets/html/IntroStyle/static/images/car_2.png' | relative_url }}" id="item-1"
                class="interpolation-image"/>
        </div>
        <div class="item item-1">
          <img src="{{ '/assets/html/IntroStyle/static/images/car_3.png' | relative_url }}" id="item-1"
               class="interpolation-image"/>
        </div>
        <div class="item item-1">
          <img src="{{ '/assets/html/IntroStyle/static/images/car_4.png' | relative_url }}" id="item-1"
               class="interpolation-image"/>
        </div>
        <div class="item item-1">
          <img src="{{ '/assets/html/IntroStyle/static/images/car_5.png' | relative_url }}" id="item-1"
               class="interpolation-image"/>
        </div>
      </div>
      <div class="content has-text-centered">
        The first left column is the query image with remaining columns showing retreival results with <span style="color: green;">green</span> colors for correct and <span style="color: rgba(222, 72, 72, 0.84);">red</span> for incorrect retrievals.
      </div>
    </div>
  </div>
</section>

<section class="section">
  <div class="container is-max-desktop">
    <div class="columns is-centered has-text-centered">
      <div class="column is-four-fifths">
        <h2 class="title is-3">Abstract</h2>
        <div class="content has-text-justified">
          <p>
          Text-to-image (T2I) models have gained widespread adoption among content creators and the general public. Gradually, there is an increasing demand for T2I models to incorporate mechanisms that prevent the generation of specific artistic styles, thereby safeguarding intellectual property rights. Existing methods for style extraction typically necessitate the collection of custom datasets and the training of specialized models. This, however, is resource-intensive, time-consuming, and often impractical for real-time applications. We present a novel, training-free framework to solve the style attribution problem, using the features produced by a diffusion model alone, without any external modules or retraining. 
          </p>
          <p>
            This is denoted as Introspective Style attribution (<span class="texttt">IntroStyle</span>) and is shown to have superior performance to state-of-the-art models for style attribution. We also introduce a synthetic dataset of Artistic Style Split (<span class="texttt">ArtSplit</span>) to isolate artistic style and evaluate fine-grained style attribution performance. Our experimental results show that our method adequately addresses the dynamic nature of artistic styles and the rapidly evolving landscape of digital art with no training overhead.
          </p>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="section">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Approach</h2>
        <div class="publication-video">
          <div class="content has-text-justified">
            Our IntroStyle approach leverages a pre-trained diffusion model for extracting style features. We encode the input image into a latent vector using the diffusion model's encoder, noise this latent to a specific timestep t, and pass the noised latent through the denoising network with a null text embedding. We then extract a feature tensor from an intermediate layer of the network, specifically from an up-block. We compute the channel-wise mean μ<sub>c</sub> and variance σ<sub>c</sub><sup>2</sup> for each channel c of this feature tensor. These statistics form our IntroStyle feature representation: f<sup>t,idx</sup>(I) = (μ<sub>1</sub>, ..., μ<sub>C</sub>, σ<sub>1</sub><sup>2</sup>, ..., σ<sub>C</sub><sup>2</sup>)<sup>T</sup>. To compare styles between images, we use the 2-Wasserstein distance between their IntroStyle representations. This simple approach proves remarkably effective for style attribution tasks.
            <br>
          </div>
          <img src="{{ '/assets/html/IntroStyle/static/images/architecture.png' | relative_url }}"
               alt="IntroStyle architecture image." height="100%"/>
          <div class="content has-text-centered">
            <span class="texttt">IntroStyle</span> computation of style similarity: channel-wise mean µ and variance σ<sup>2</sup> are computed for the identified style layers. Then a distance metric, 2-Wassertein Distance, can be used to measure styles between a pair of images.
          </div>
        </div>
      </div>
    </div>

    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Artistic Style Split (<span class="texttt">ArtSplit</span>) Dataset</h2>
        <div class="content has-text-justified">
          To address the limitations of existing datasets for fine-grained evaluation of style retrieval, we propose the Artistic Style Split (<span class="texttt">ArtSplit</span>) dataset. This was created with the prompt-image pairs of the 2 most recognized works of 50 prominent artists from the LAION Aesthetic Dataset. For each of the two paintings, ChatGPT-4o was asked to generate a "style" specification and a "semantic" description, such that there is no style information in the semantic description and vice-versa. Stable Diffusion v2.1 was then used with a combination of two prompts, "style" and "semantic," to synthesize a reference image dataset. With 50 artists and 100 paintings, this led to 50 X 100 = 5,000 prompt combinations. A set of 12 images was sampled per combination, yielding 60,000 images in total. The procedure is detailed in Supplemental Section 4.
        </div>
        <img src="{{ '/assets/html/IntroStyle/static/images/artsplit_sample.png' | relative_url }}"
             alt="ArtSplit dataset image." height="100%"/>
        <div class="content has-text-centered">
           Artistic Style Split (<span class="texttt">ArtSplit</span>) Dataset samples. Each row shows images generated with the same style, and each column with the same semantics.
        </div> 
      </div>
    </div>

    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Comparision with state-of-the-art models</h2>
        <div class="content has-text-justified">
          We compare our retreival method with state-of-the-art models for style attribution. We also use the <span class="texttt">ArtSplit</span> dataset to evaluate the performance of our method against the baseline models. The results show that our method outperforms the baseline models in fine-grained style attribution tasks.
        </div>
        <img src="{{ '/assets/html/IntroStyle/static/images/wikiart_results.png' | relative_url }}"
             alt="Retreival on Wikiart." height="100%"/>
        <div class="content has-text-centered">
           Wikiart retrieval results.
        </div> 
        <img src="{{ '/assets/html/IntroStyle/static/images/style_artsplit.png' | relative_url }}"
             alt="Retreival on ArtSplit." height="100%"/>
        <div class="content has-text-centered">
           <b>Style-based</b> Artistic Style Split (<span class="texttt">ArtSplit</span>) retrieval results. We show the ranked images for a fixed semantic for isolating stylistic variations.
        </div>
        <img src="{{ '/assets/html/IntroStyle/static/images/semantic_artsplit.png' | relative_url }}"
             alt="Retreival on ArtSplit." height="100%"/>
        <div class="content has-text-centered">
           <b>Semantic-based</b> Artistic Style Split (<span class="texttt">ArtSplit</span>) retrieval results. The results suggest that our retrieval emphasizes styles rather than semantic content.
        </div>
      </div>
    </div>
  </div>
</section>

<section class="section" id="BibTeX">
  <div class="container is-max-desktop content">
    <h2 class="title">BibTeX</h2>
    <pre><code>@article{kumar2024introstyle,
  author    = {Kumar, Anand and Mu, Jiteng and Vasconcelos, Nuno},
  title     = {IntroStyle: Training-Free Introspective Style Attribution using Diffusion Features},
  journal   = {arXiv preprint arXiv: 2412.14432},
  year      = {2024},
}</code></pre>
  </div>
</section>

<footer class="footer">
  <div class="container">
    <div class="content has-text-centered">
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