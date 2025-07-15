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



<!--   -->
<!-- Research -->
<!--   -->

<h2 id="research">Research</h2>

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

<p class="mytext"><strong>DNA methylation biomarkers in acute coronary syndrome (blood-derived cfDNA)</strong></p>

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
<p class="mytext"><strong>DNA methylation profiling in neuroblastoma (solid tissues and urine-derived cfDNA)</strong></p>

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









<!--   -->
<!-- Open source software -->
<!--   -->

<h2 id="opensource">Open source software</h2>


<!-- Genomation-->

<p class="mytext">
<div class="software-block">
  <img src="img/genomation.png" alt="Genomation logo" class="software-logo">

  <div class="software-text">
    <p><em>genomation</em> – a Bioconductor R package designed to simplify genomic feature and interval analysis. It includes functions for reading BED/GFF files as GRanges, summarizing features over regions, creating enrichment plots or heatmaps, and annotating regions with exons, introns, or promoters.</p>

  </div>
</div>
</p>

<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
  <a href="https://github.com/BIMSBbioinfo/genomation" target="_blank">https://github.com/BIMSBbioinfo/genomation</a>,
  developed in the team of Dr. Altuna Akalin at Bioinformatics and Omics Data Science Platform at 
<a href="https://www.mdc-berlin.de/bioinformatics" target="_blank">MDC BIMSB.</a>
</p>



<!-- Pigx -->
<div class="software-block">
  <img src="img/pigx.png" alt="PiGx logo" class="software-logo">

  <div class="software-text">
    <p><em>PiGx</em> – a collection of genomics pipelines implemented using Snakemake, Python, and R. Each pipeline is easily configured with a sample sheet and a simple settings file. PiGx generates comprehensive, interactive HTML reports that summarize key findings from your samples.</p>
  </div>
</div>

<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
  <a href="https://github.com/BIMSBbioinfo/pigx" target="_blank">
    https://github.com/BIMSBbioinfo/pigx</a>,
  developed in the team of Dr. Altuna Akalin at Bioinformatics and Omics Data Science Platform at 
<a href="https://www.mdc-berlin.de/bioinformatics" target="_blank">MDC BIMSB.</a>
</p>


<!-- Motif activity -->

<div class="software-block">
  <img src="img/motifActivity.png" alt="motifActivity logo" class="software-logo">

  <div class="software-text">
    <p><em>motifActivity</em> – an R package for identifying key transcription factors (TFs) responsible for changes in gene expression or epigenetic marks across samples. It predicts TF activity profiles using input data from RNA-seq, BS-seq, ChIP-seq, ATAC-seq, and similar methods, combined with a set of DNA motifs.</p>
  </div>
</div>

<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
  <a href="https://github.com/katwre/motifActivity" target="_blank">
    https://github.com/katwre/motifActivity</a>,
  developed in the team of Dr. Altuna Akalin at Bioinformatics and Omics Data Science Platform at 
<a href="https://www.mdc-berlin.de/bioinformatics" target="_blank">MDC BIMSB.</a>

</p>









<!--   -->
<!-- Freelance -->
<!--   -->

<!-- Prioritization of therapeutic targets in clinical trials  -->
<p class="mytext"><strong>4.1 Prioritization of therapeutic targets in clinical trials</strong></p>

<h3 class="mytext"><strong>Visualization and Statistical Analysis of Biomarkers</strong></h3>

<p class="mytext">
We developed interactive visualizations, including oncoprints, to highlight key biomarkers in patients with limited treatment options. These visual summaries help uncover genomic alterations and support identifying new therapeutic targets.
</p>

<p class="mytext">
We focused on patients from clinical trial databases facing poor outcomes or lacking effective therapies. Our statistical analyses, including survival analysis, demonstrate the clinical relevance of nominated targets.
</p>

<p class="mytext" style="text-align:center;">
  <img src="img/oncoprint_modified.png" style="max-width:65%;">
  <img src="img/survival_analysis.png" style="max-width:65%;">
</p>

<p class="mytext" style="text-align:center; font-size: 14px; color: #555;">Figure: Example of biomarker visualization and survival analysis.
</p>


<h3 class="mytext"><strong>Machine learning for target identification</strong></h3>

<p class="mytext">
To prioritize therapeutic targets, we applied <a href="https://cseweb.ucsd.edu/~elkan/posonly.pdf" target="_blank">Positive and Unlabeled (PU) learning</a>, ideal for cases where only confirmed targets are known. PU classifiers helped distinguish potential targets using gene expression, mutations, and therapy annotations.
</p>
<p class="mytext" style="text-align:center;">
  <img src="img/PUlearning.png" style="max-width:100%;">
</p>
<p class="mytext" style="text-align:center; font-size: 14px; color: #555;">
Figure: PU learning principle (figure adapted from <a href="https://techblog.ing.pl/blog/podstawy-positive-unlabeled-learning" target="_blank">a blogpost</a>).
</p>


<p class="mytext">
  Additionally, we used autoencoders (PyTorch) to uncover hidden patterns and prioritize key molecular features in an unsupervised way.
  </p>
<p class="mytext" style="text-align:center;">
  <img src="img/autoencoder_TFs.png" style="max-width:110%;max-height:90%">
</p>
<p class="mytext" style="text-align:center; font-size: 14px; color: #555;">
Figure: Autoencoder workflow and latent space visualization using t-SNE.
</p>




<!-- 5.2 Web app feature development  -->
<p class="mytext"><strong>4.2 Web app feature development</strong></p>

<p class="mytext">
  I contributed to enhancing the 
  <a href="https://igv.org/app/" target="_blank">IGV web application</a>, 
  an interactive tool for visual exploration of genomic data 
  (<a href="https://github.com/igvteam/igv-webapp" target="_blank">source code</a>).
  Built with JavaScript and Python, this tool allows visualization of both public and in-house datasets.
  </p>
  
  <ul class="mytext" style="list-style-type: disc; margin-left: 110px;">
    <li>Enabled dynamic visualization of new in-house genomic datasets.</li>
    <li>Added highlighting of genomic regions of interest (e.g., genetic variants).</li>
    <li>Developed new display options for RefSeq and GENCODE annotations:
      <ul>
        <li>Collapse/expand all transcript isoforms.</li>
        <li>Extend selected gene isoforms for detailed view.</li>
        <li>Added controls to adjust track widths for optimal display.</li>
      </ul>
    </li>
    <li>Linked visualized tracks to their source databases.</li>
    <li>Implemented command-line tool for automated snapshots of defined genes or regions.</li>
  </ul>
  
  
  <div style="text-align: center;">
    <img src="img/igv_original.png" style="max-width: 70%; height: auto;">
    <div class="mytext" style="font-size: 14px; color: #555;">
      Figure: Example IGV web app view showing genomic data tracks.
    </div>
  </div>




<!--   -->
<!-- Side projects -->
<!--   -->

<h2 id="sideprojects">Side projects</h2>


<!-- Protein Folding -->
<div class="software-block">
<div class="software-text">
<p>
  <em>Protein Folding in the HP Model</em> - implementation of simulated annealing and replica exchange Monte Carlo algorithm for protein folding in the HP model in Python and NumPy. The HP model simplifies protein folding by using hydrophobic (H) and polar (P) amino acids on a square lattice. Metropolis–Hastings algorithm enables sampling protein configurations based on the Boltzmann distribution.
</p>
</div>
</div>

<div style="text-align: center;">
  <img src="img/HPmodel.png" width="200" height="200">
  <p class="mytext" style="text-align: center;font-size: 0.9em; color: #666;">Figure: Lattice HP model showing global energy.</p>
</div>
<p class="mytext" style="text-align: center;font-family: 'Cormorant Garamond', serif;">
<a href="https://github.com/katwre/bioinformatics-projects/tree/master/Molecular_Dynamics" target="_blank">https://github.com/katwre/bioinformatics-projects/tree/master/Molecular_Dynamics</a>
</p>

<hr>

<!-- Genome Assembly -->
<div class="software-block">
  <div class="software-text">
  <p>
    <em>Genome Assembly Using de Bruijn Graph</em> - implementation of de Bruijn graph-based genome assembly with Eulerian walk to reconstruct DNA sequences from k-mers. Includes short-read assembly principles based on publications by Compeau et al. (2011) and Pevzner et al. (2001)
  </p>
  </div>
  </div>
<div style="text-align: center;">
  <img src="img/debrujin.png" style="max-width: 300px; width: 70%;">
  <p class="mytext" style="text-align: center;font-size: 0.9em; color: #666;">Figure: De Bruijn graph.</p>
</div>
<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
<a href="https://github.com/katwre/bioinformatics-projects/tree/master/genome_assembly" target="_blank">https://github.com/katwre/bioinformatics-projects/tree/master/genome_assembly</a>
</p>

<hr>

<!-- Sudoku -->
<div class="software-block">
  <div class="software-text">
  <p>
    <em>Sudoku</em> - a simple Sudoku game implemented in JavaScript and JQuery. </p>
  </div>
  </div>
<div style="text-align: center;">
  <img src="img/sudoku.png" width="400" height="300">
</div>
<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
<a href="https://github.com/katwre/sudoku" target="_blank">https://github.com/katwre/sudoku</a>
</p>

<hr>

<!-- Minesweeper -->

<div class="software-block">
  <div class="software-text">
  <p>
    <em>Minesweeper</em> - classic Minesweeper game implemented in Java using SWING and AWT libraries. </p>
  </div>
  </div>
<div style="text-align: center;">
  <img src="img/minesweeper.png" width="200" height="230">
</div>
<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
<a href="https://github.com/katwre/Minesweeper" target="_blank">https://github.com/katwre/Minesweeper</a>
</p>

<hr>

<!-- Django Web-Services -->
<p class="mytext"><strong>Django-Based Web Services</strong></p>
<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
Django-based server for Multiple Sequence Alignment (MSA) visualization - <a href="https://github.com/freesci/MSA-vis-project" target="_blank">https://github.com/freesci/MSA-vis-project</a>

</p>
<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
Mobile application using Django, manifesto app, and localStorage - <a href="https://github.com/katwre/phone_application" target="_blank">https://github.com/katwre/phone_application</a>
</p>


<hr>

<!-- Discover Career Match -->
<p class="mytext"><strong>Discover Your Career Match</strong></p>
<p class="mytext">
Interactive tool that matches careers to users based on their personality profile (Big Five personality traits). Runs directly in the browser via Pyodide.
</p>

<div style="text-align: center;">
  <img src="img/personalities.png" alt="PCA plot of careers based on personality traits" style="max-width: 70%; max-height: 70%; border: 1px solid #ccc; box-shadow: 2px 2px 6px #ddd;">
  <p class="mytext" style="text-align: center;font-size: 0.9em; color: #666;">Figure: PCA plot showing career matches based on personality profile.</p>
</div>
<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
  <a href="https://github.com/katwre/Personalities" target="_blank">https://github.com/katwre/Personalities</a>
  </p>


