---
layout: page
title: ""
permalink: /projects/
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




<!--   -->
<!-- Research -->
<!--   -->

<h2 id="research">Projects</h2>


<div class="toc-wrapper">
<ol class="toc-list">
  <li>
    <a href="#research">Research</a>
    <ol>
      <li><a href="#genomics">Bias interpretation in genomics</a></li>
      <li><a href="#cfDNA">Liquid biopsy epigenetics in disease</a></li>
    </ol>
  </li>
  <li><a href="#opensource">Open source software</a></li>
  <li><a href="#freelance">Freelance</a>
    <ol>
      <li><a href="#target">Prioritization of therapeutic targets in clinical trials</a></li>
      <li><a href="#igv">Web app feature development</a></li>
    </ol>
  </li>
  <li><a href="#sideprojects">Side projects</a></li>
</ol>
</div>


<!-- Bias detection and interpretation in genomics experiment -->
<p class="mytext" id="genomics"><strong>Bias interpretation in genomics</strong></p>

<p class="mytext">
  We used machine learning models - elastic net regression and principal component analysis (PCA)-
  to investigate genomic regions called 'HOT regions' 
  which appear to attract unusually high numbers of proteins and 
  are likely 
  <a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC4538825/" target="_blank">technical artifacts</a>
  of chromatin immunoprecipitation followed by sequencing 
  (<a href="https://www.nature.com/articles/nrg2641" target="_blank">ChIP-seq</a>) experiments.
</p>





<p class="mytext">
  While factors like antibody quality and chromatin interactions are known to affect ChIP-seq reliability, 
  our study revealed that GC- and CpG-rich sequences, 
  <a href="https://www.nature.com/articles/npp2012112" target="_blank">DNA methylation</a>,
   and RNA:DNA hybrids 
  (<a href="https://www.nature.com/articles/s41580-022-00474-x" target="_blank">R-loops</a>)
   also contribute to these artifacts across species. This work shows how machine learning can uncover hidden biases in 
   genomic data and improve experimental interpretation.
</p>


<p class="mytext">

  <figure style="text-align: center; max-width: 700px; margin: 0 auto;">
    <img src="/img/hot.png" alt="HOT regions figure" style="width: 80%; height: 80%;">
  
    <figcaption class="mytext" style="text-align: center; font-family: 'Georgia', serif; font-size: 14px; color: #555; margin-top: 10px;">
      Figure: Unexpected ChIP-seq signals appear in HOT regions even without the target protein (KO ChIP-seq). 
      The barplot shows how often these regions are detected as bound - 
      HOT regions correspond to the top 1% of genomic regions with the highest protein binding signals (99th percentile).


    </figcaption>
  </figure>
</p>

  <p class="mytext">
    <a href="https://doi.org/10.1093/nar/gkv681" target="_blank">
      Publication: Wreczycka K et al, Nucleic Acids Research, 2019
    </a>
  </p>
  


<!-- cfDNA methylation biomarkers in acute coronary syndrome -->
<p class="mytext" id="cfDNA"><strong>Liquid biopsy epigenetics in disease</strong></p>

<p class="mytext"><span style="color:#505050; font-weight:bold;">DNA methylation biomarkers in acute coronary syndrome (blood-derived cfDNA)</span></p>

<p class="mytext">
  We explored circulating cell-free DNA (<a href="https://doi.org/10.1038/s41571-020-00457-x" target="_blank">cfDNA</a>) methylation 
  as a non-invasive biomarker for acute coronary syndrome (ACS),
  based on the principle that damaged tissues release DNA into the bloodstream.
</p>

<p class="mytext">
  Using cfDNA methylation profiles, we differentiated ACS subtypes and identified cell type-specific DNA methylation
  markers to trace the origin of cfDNA. Hundreds of methylation markers linked to cardiovascular conditions and inflammation 
  were identified and validated in an independent cohort, highlighting the potential of cfDNA methylation for ACS diagnosis.
</p>

<p class="mytext">
  <figure style="text-align: center; max-width: 700px; margin: 0 auto;">
    <img src="/img/cfndaacs.png" alt="HOT regions figure" style="width: 30%; height: 30%;">
  
    <figcaption class="mytext" style="text-align: center; font-family: 'Georgia', serif; font-size: 14px; color: #555; margin-top: 10px;">
      Figure: PCA of 254 differentially methylated regions linked to ACS severity using linear models.
    </figcaption>
  </figure>
</p>

<p class="mytext">
  <a href="https://doi.org/10.1093/nargab/lqad061" target="_blank">
  Publication: Rafael R C Cuadrat et al, NAR Genomics and Bioinformatics, 2023
  </a>
</p>




<!-- DNA methylation in neuroblastoma -->
<p class="mytext"><span style="color:#505050; font-weight:bold;">DNA methylation profiling in neuroblastoma (solid tissues and urine-derived cfDNA)</span></p>

<p class="mytext">
  Neuroblastoma is a pediatric cancer ranging from mild to aggressive forms. While genetic changes explain some variability, 
  we showed that DNA methylation plays a key role in its progression. 
  In collaboration with Charité Hospital (Berlin), we analyzed primary tumor tissues and urine cfDNA 
  using bisulfite-seq and RNA-seq, identifying methylation patterns 
  distinguishing high- and low-risk tumors. We also linked MYCN-driven 
  methylation changes to disrupted transcription factor networks, highlighting potential targets for therapies.
</p>

<p class="mytext" style="text-align: center;">
  <img src="/img/neuroblastoma_clustering.png" alt="Neuroblastoma clustering" style="width: 80%; max-width: 600px;">
</p>
<p class="mytext" style="text-align: center; font-size: 14px; color: #555;">
  Figure: Methylation-based clustering of neuroblastoma patients using differentially methylated CpGs.
</p>

<!-- 
<p class="mytext" style="text-align: center;">
  <img src="/img/neuroblastoma_networks.png" alt="Neuroblastoma networks" style="width: 60%; max-width: 500px;">
</p>
<p class="mytext" style="text-align: center; font-size: 14px; color: #555;">
  Figure: (A) Regulatory networks based on motif activity in MYCN-amplified and high-risk tumors. 
  (B) Enriched gene pathways including transcription factors binding to E-box DNA motifs.
</p>
-->






