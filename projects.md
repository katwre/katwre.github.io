---
layout: page
title: ""
---

<style>

h1, .page-title {
  font-family: 'Cormorant Garamond', serif;
    font-size: 36px;
    font-weight: bold;
    color: black;
    text-align: center;
    margin-bottom: 10px;
}
h2 {
  font-family: 'Cormorant Garamond', serif;
    font-size: 36px;
    color: black;
    line-height: 1.6;
    text-align: justify;           /* Justify the text itself */
    max-width: 600px;              /* Restrict paragraph width */
    margin: 0 auto 40px auto;      /* Center the block itself */
    padding: 0 20px;               /* Optional: adds side padding for extra visual balance */
}

.degrees {
  font-family: 'Cormorant Garamond', serif;
    font-size: 16px;
    text-transform: uppercase;
    letter-spacing: 1px;
    text-align: center;
    color: black;
    margin-bottom: 30px;
}

.intro-bio {
  font-family: 'Inter', sans-serif;
    font-size: 16px;
    color: black;
    line-height: 1.6;
    text-align: justify;           /* Justify the text itself */
    max-width: 600px;              /* Restrict paragraph width */
    margin: 0 auto 40px auto;      /* Center the block itself */
    padding: 0 20px;               /* Optional: adds side padding for extra visual balance */
}


.social-icons {
    text-align: center;
    margin: 15px 0 25px 0;
}

.social-icons a {
    display: inline-block;
    font-size: 28px; /* adjust icon size */
    color: #990033;    /* or gray if preferred */
    margin: 0 10px;  /* space between icons */
    text-decoration: none;
}

.social-icons a:hover {
    color: #555555;
}

.mytext {
  font-family: 'Inter', sans-serif;
    font-size: 16px;
    color: black;
    line-height: 1.6;
    text-align: justify;           /* Justify the text itself */
    max-width: 600px;              /* Restrict paragraph width */
    margin: 0 auto 40px auto;      /* Center the block itself */
    padding: 0 20px;               /* Optional: adds side padding for extra visual balance */

}

ol {
  font-family: 'Georgia', serif;
    font-size: 16px;
    
}
.main-content ol {
  font-family: 'Georgia', serif;
  font-size: 16px;
  margin-left: 20px;
}

ol li a {
    color: #80002a; /* your accent color */
    text-decoration: none;
}

ol li a:hover {
    text-decoration: underline;
}
/* Main ToC block */
.toc-wrapper {
    max-width: 600px;
    margin: 0 auto 40px auto;
    padding: 0 20px;
    text-align: left;
}

.toc-list {
    list-style: none;
    counter-reset: item;
    font-family: 'Georgia', serif;
    font-size: 16px;
    padding-left: 0;
}

/* List items and numbering */
.toc-list li {
    display: block;
    margin: 5px 0;
    counter-increment: item;
}

.toc-list li:before {
    content: counters(item, ".") " ";
    margin-right: 5px;
    font-weight: normal;
}

/* Nested list handling */
.toc-list ol {
    counter-reset: item;
    list-style: none;
    padding-left: 20px;
    margin: 5px 0;
}

/* Links inside the ToC */
.toc-list a {
    text-decoration: underline;
    color: #80002a;
}

.toc-list a:hover {
    color: black;
}

.software-block {
  display: flex;
  align-items: center;
  max-width: 600px;
    margin: 0 auto 40px auto;
    padding: 0 20px;
    text-align: left;
}

.software-logo {
  width: 110px;
  height: auto;
  margin-right: 20px;
}

.software-text {
  font-family: 'Cormorant Garamond', serif;
  font-size: 18px;
  color: black;
  line-height: 1.5;
}

.software-text a {
  color: #80002a;
  text-decoration: none;
}

.software-text a:hover {
  text-decoration: underline;
}

.emphasize {
  color: #80002a;  /* subtle burgundy or your brand color */
  font-weight: 500; /* medium weight for softer emphasis */
}


</style>

<p class="mytext">
Here’s a glimpse of my portfolio.
</p>

<div class="mytext">

  <h3>Statistical Analysis</h3>
  <p>I employed a wide range of statistical techniques to extract meaningful insights from complex datasets, including:</p>
  <ul>
  <li><span class="emphasize">Survival Analysis</span>: Kaplan-Meier estimator, Cox proportional hazards model</li>
  <li><span class="emphasize">Regression Analysis</span>: Linear regression and other predictive models</li>
  <li><span class="emphasize">Classification Methods</span>: Logistic regression, elastic net, random forests, SVMs, and positive-unlabeled learning</li>
  <li><span class="emphasize">Unsupervised Methods</span>: Hierarchical clustering, PCA, MOFA, and autoencoders</li>
</ul>



  <h3>Omics Data Analysis</h3>
  <p>
    I specialize in leveraging advanced statistical methods and developing cutting-edge software tools to process 
    and analyze large-scale sequencing datasets. These innovations enable the discovery of meaningful patterns and relationships 
    across diverse omics datasets, paving the way for robust hypothesis generation and data-driven insights.
  </p>


  <p>In my projects, I integrated multi-omics data from a variety of sources, including:</p>
<ul>
  <li><span class="emphasize">Gene expression</span> data (RNA-seq, scRNA-seq)</li>
  <li><span class="emphasize">DNA methylation</span> profiles (Bisulfite-seq, RRBS, methylation arrays)</li>
  <li><span class="emphasize">Open chromatin</span> regions (ATAC-seq)</li>
  <li><span class="emphasize">Transcription factor binding sites</span> (ChIP-seq)</li>
  <li>Data from <span class="emphasize">specialized protocols</span> and methods, such as DRIP-seq and RDIP-seq, for detecting DNA-RNA hybrids</li>
  <li>Information on <span class="emphasize">therapies</span>, <span class="emphasize">drugs</span>, and <span class="emphasize">biomarkers</span> from internal and external clinical trial databases</li>
</ul>

  <p>By combining these diverse data types, I created comprehensive models that contribute to understanding complex biological systems.</p>


</div>

