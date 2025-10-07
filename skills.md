---
layout: page
title: 
permalink: /skills/
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


<h2  style="font-family: 'Cormorant Garamond', serif;">
  Skills
</h2>

<!--
<h2  style="font-family: 'Cormorant Garamond', serif;">
  Data science & omics
</h2>

<div class="mytext">

  <p>I've employed a wide range of statistical techniques to extract meaningful insights from complex datasets, including:</p>
  <ul>
  <li><span class="emphasize">Survival Analysis</span>: Kaplan-Meier estimator, Cox proportional hazards model</li>
  <li><span class="emphasize">Regression Analysis</span>: Linear regression, elastic net/ridge/LASSO</li>
  <li><span class="emphasize">Classification Methods</span>: Logistic regression, random forests, XGBoost, SVM</li>
  <li><span class="emphasize">Unsupervised Methods</span>: Hierarchical clustering, PCA, MOFA, NMF</li>
  <li><span class="emphasize">Deep learning</span>: variational autoencoders (VAEs), CNNs, transformers, retrieval-augmented generation (RAG)), federated learning </li>
</ul>
-->

<!--
  <h3>Omics data analysis</h3>
  
  <p>
    My work focuses on analyzing large-scale sequencing data with statistical methods and software tools to uncover patterns across various omics datasets, including:
  </p>
<ul>
  <li><span class="emphasize">Gene expression</span> data (RNA-seq, scRNA-seq)</li>
  <li><span class="emphasize">DNA methylation</span> profiles (Bisulfite-seq, RRBS, methylation arrays)</li>
  <li><span class="emphasize">Open chromatin</span> regions (ATAC-seq)</li>
  <li><span class="emphasize">Transcription factor binding sites</span> (ChIP-seq)</li>
  <li>Data from <span class="emphasize">specialized protocols</span> and methods, such as DRIP-seq and RDIP-seq, for detecting DNA-RNA hybrids</li>
  <li>Information on <span class="emphasize">therapies</span>, <span class="emphasize">drugs</span>, and <span class="emphasize">biomarkers</span> from internal and external clinical trial databases</li>
</ul>

</div>
-->



<!--Soft skills:-->


<ul>

<li><span class="emphasize">Collaboration & Communication</span>: </li>

<ul>
<li>Working in an independent manner and also in cross-functional teams (clinicians, wet-lab scientists, data scientists, software engineers, UX/UI designers)</li>
<li>Gathering, evaluating and synthesizing of information into articles</li>
<li>Project management and mentoring</li>
<li>Good at communication and presentation skills</li>
<li>Good at problem solving and adaptability</li>
<li>Curious and loves to learn new things</li>
</ul>

</ul>



<!--Technical skills:-->


<ul>
  <li><span class="emphasize">Programming &amp; Tools</span>: 
  
  <ul>
  <li>Python - NumPy, pandas, scikit-learn, seaborn, PyTorch, Matplotlib, Plotly, Biopython</li>
  <li>R - CRAN, Bioconductor</li>
  <li>RMarkdown, Jupyter Notebooks</li>
  <li>unit testing - R/testthat, Python/unittest/pytest</li>
  <li>bash</li>

  </ul>
  
  </li>
  
  <li><span class="emphasize">Machine Learning</span>: 
   <ul>
    <li>Statistical tests: incl. t-tests, Wilcoxon</li>
    <li>Regression: incl. linear regression, logistic regression, Cox/survival analysis, elastic net/ridge/LASSO</li>
    <li>Classification: incl. random forests, XGBoost, SVM, Linear Discriminant Analysis (LDA)</li>
    <li>Clustering: K-means, EM algorithm</li>
    <li>Probabilistic models: Hidden Markov models (HMMs), linear Gaussian state-space models</li>
    <li>Dimensionality reduction & factorization: PCA, t-SNE, MOFA, NMF</li>
    <li>Sampling &amp; optimization: replica exchange Monte Carlo</li>
    <li>Deep learning: variational autoencoders (VAEs), CNNs, transformers, retrieval-augmented generation (RAG), LLMs</li>
    <li>Federated learning</li>
  </ul>
  
  </li>
  
  <li><span class="emphasize">MLOps</span>: 
  <ul>
  <li>Workflow languages - Nextflow, Snakemake</li>
  <li>Docker, Singularity</li>
  <li>SLURM, Grid Engine, Kubernetes</li>
  <li>AWS, DigitalOcean</li>  </ul>
  </li>

  <li><span class="emphasize">Databases</span>: MySQL, SQLite, PostgreSQL</li>
  
  <li><span class="emphasize">Version Control &amp; Software Management</span>: Linux/Unix systems, git, svn, conda, GNU Guix</li>
  
  <li><span class="emphasize">Web Frameworks</span>: Django, CSS, JavaScript, HTML, jQuery, PHP</li>
  
</ul>



