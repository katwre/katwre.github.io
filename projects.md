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
<!-- list of chapters -->
<!--   -->


<h2 id="projects">Portfolio</h2>


<div class="toc-wrapper">
<ol class="toc-list">
    <li>
      <strong><a href="#research">Research</a></strong>
      <ol>
        <li><a href="#genomics">Bias interpretation in genomics</a></li>
        <li><a href="#cfDNA">Liquid biopsy epigenetics in disease</a></li>
      </ol>
    </li>
    <li>
      <strong><a href="#opensource">Open Source Software</a></strong>
    </li>
    <li>
      <strong><a href="#freelance">Freelance</a></strong>
      <ol>
        <li><a href="#target">ML/AI prioritization of therapeutic targets in clinical trials</a></li>
        <li><a href="#igv">Web app feature development</a></li>
      </ol>
    </li>
    <li>
      <strong><a href="#sideprojects">Side Projects</a></strong>
      <ol>
        <li><a href="#survival">Survival analysis using gene expression & clinical data (Cox models)</a></li>
        <li><a href="#dlomics">Deep learning for xray images and omics (CNNs, transfer learning, VAE, NMF, BERT)</a></li>
        <li><a href="#llm">LLM-based assistant for bioinformatics queries</a></li>
        <li><a href="#algorithms">Computational biology & algorithms</a></li>
        <ol>
        <li><a href="#rmc">Protein folding - Monte Carlo</a></li>
        <li><a href="#debrujn">Genome assembly - de Bruijn graph, euler walk</a></li>
        <li><a href="#felnni">Evolutionary tree estimation - Felsenstein & NNI</a></li>
        <li><a href="#binomial">Regulatory DNA discovery - MSA & binomial enrichment</a></li>
        </ol> 
        <li><a href="#games">Games: Sudoku (JavaScript) and Minesweeper (Java)</a></li>
        <li><a href="#django">Django web services (Multiple Sequence Alignment visualization and mobile app)</a></li>
        <li><a href="#pyodine">In-browser Python career-matching tool (Pyodine)</a></li>
      </ol>
    </li>
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




<!--   -->
<!-- Open source software -->
<!--   -->

<h2 id="opensource">Open source software</h2>


<!-- Genomation-->

<div class="software-block mytext">
  <img src="{{ '/img/genomation.png' | relative_url }}" alt="Genomation logo" class="software-logo">
  <div class="software-text">
    <p><em>genomation</em> – a Bioconductor R package designed to simplify genomic feature and interval analysis. It includes functions for reading BED/GFF files as GRanges, summarizing features over regions, creating enrichment plots or heatmaps, and annotating regions with exons, introns, or promoters.</p>
  </div>
</div>


<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
  <a href="https://github.com/BIMSBbioinfo/genomation" target="_blank">https://github.com/BIMSBbioinfo/genomation</a>,
  developed in the team of Dr. Altuna Akalin at Bioinformatics and Omics Data Science Platform at 
<a href="https://www.mdc-berlin.de/bioinformatics" target="_blank">MDC BIMSB.</a>
</p>



<!-- Pigx -->
<div class="software-block">
    <img src="{{ '/img/pigx.png' | relative_url }}" alt="pigx logo" class="software-logo">

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
  <img src="{{ '/img/motifActivity.png' | relative_url }}" alt="motifActivity logo" class="software-logo">


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

<h2 id="freelance">Freelance</h2>


<!-- Prioritization of therapeutic targets in clinical trials  -->
<p class="mytext" id="target"><strong>Prioritization of therapeutic targets in clinical trials</strong></p>

<p class="mytext"><span style="color:#505050; font-weight:bold;">Visualization and survival analysis of biomarkers</span></p>

<p class="mytext">
We developed interactive visualizations, including oncoprints, to highlight key biomarkers in patients with limited treatment options. These visual summaries help uncover genomic alterations and support identifying new therapeutic targets.
</p>

<p class="mytext">
We focused on patients from clinical trial databases facing poor outcomes or lacking effective therapies. Our statistical analyses, including survival analysis, demonstrate the clinical relevance of nominated targets.
</p>

<p class="mytext" style="text-align:center;">
  <img src="{{ '/img/oncoprint_modified.png' | relative_url }}" style="max-width:65%;">
  <img src="{{ '/img/survival_analysis.png' | relative_url }}" style="max-width:65%;">
</p>

<p class="mytext" style="text-align:center; font-size: 14px; color: #555;">Figure: Example of biomarker visualization and survival analysis.
</p>


<p class="mytext" id="mltarget"><span style="color:#505050; font-weight:bold;">Machine learning/AI for target identification</span></p>

<p class="mytext">
To prioritize therapeutic targets, we applied <a href="https://cseweb.ucsd.edu/~elkan/posonly.pdf" target="_blank">Positive and Unlabeled (PU) learning</a>, ideal for cases where only confirmed targets are known. PU classifiers helped distinguish potential targets using gene expression, mutations, and therapy annotations.
</p>
<p class="mytext" style="text-align:center;">
  <img src="{{ '/img/PUlearning.png' | relative_url }}" style="max-width:100%;">
</p>

<p class="mytext" style="text-align:center; font-size: 14px; color: #555;">
Figure: PU learning principle (figure adapted from <a href="https://techblog.ing.pl/blog/podstawy-positive-unlabeled-learning" target="_blank">a blogpost</a>).
</p>


<p class="mytext">
  Additionally, we utilized autoencoders to uncover hidden patterns and prioritize key molecular features in an unsupervised way.
  </p>
<p class="mytext" style="text-align:center;">
  <img src="{{ 'img/variational-autoencoder.png' | relative_url }}" style="max-width:70%;max-height:90%">
</p>


<p class="mytext" style="text-align:center; font-size: 14px; color: #555;">
Figure: Schematic of a Variational Autoencoder (figure adapted from <a href="https://avandekleut.github.io/vae/" target="_blank">a blogpost</a>).
</p>




<!-- Web app feature development  -->
<p class="mytext" id="igv"><strong>Web app feature development</strong></p>

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
      <img src="{{ 'img/igv_original.png' | relative_url }}" style="max-width: 70%; height: auto;">

    <div class="mytext" style="font-size: 14px; color: #555;">
      Figure: Example IGV web app view showing genomic data tracks.
    </div>
  </div>




<!--   -->
<!-- Side projects -->
<!--   -->


<h2 id="sideprojects">Side projects</h2>


<!-- survival  -->
<p class="mytext" id="survival"><strong>Survival analysis using gene expression & clinical data (Cox models)</strong></p>


<p class="mytext">
I developed several survival models to predict the risk of mortality or relapse in newly diagnosed multiple myeloma patients, using baseline clinical and/or gene expression data.The workflow involved RNA-seq preprocessing, unsupervised exploratory analysis (PCA, clustering), and multiple survival modeling strategies - Cox regression, random survival forests, LASSO-based feature selection, and pathway-informed models - evaluated using the C-index.

</p>

<div style="text-align: center;">
  <img src="{{ 'img/survival_classification.png' | relative_url }}" width="550" height="300">
  <p class="mytext" style="text-align: center;font-size: 0.9em; color: #666;">Figure: C-index comparison of multiple survival models.</p>
</div>

<div style="text-align: center;">
  <img src="{{ 'img/surival_probability.png' | relative_url }}" width="300" height="300">
  <p class="mytext" style="text-align: center;font-size: 0.9em; color: #666;">Figure: Kaplan–Meier plot of the best performing model.</p>
</div>

<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
<a href="https://github.com/katwre/survival_analysis/tree/main/" target="_blank">https://github.com/katwre/survival_analysis/tree/main/</a>
</p>





<!--   -->
<!-- DL in omics  -->
<!--   -->


<p class="mytext" id="dlomics"><strong>Deep learning for xray images and omics (CNNs, transfer learning, VAE, NMF, BERT)</strong></p>


<!-- cnn  -->
<p class="mytext" id="cnn"><span style="color:#505050; font-weight:bold;">CNNs and transfer learning for image classification tasks based on chest X-rays</span></p>

<p class="mytext">
I applied convolutional neural networks (CNNs) to classify chest X-ray images using both 224×224 and 64×64 pixel inputs, aiming to explore whether lightweight models can retain sufficient diagnostic power for image-based classification tasks. In addition to training a baseline CNN from scratch, I employed transfer learning with pretrained convolutional backbones such as ResNet to evaluate whether pretrained models could further enhance classification performance on chest X-ray images.
</p>

<div style="display: flex; justify-content: center; gap: 20px;">

  <div style="text-align: center;">
    <img src="{{ 'img/xray.jpeg' | relative_url }}" width="200" height="200">
    <p style="font-size: 0.9em; color: #666;">Healthy</p>
  </div>

  <div style="text-align: center;">
    <img src="{{ 'img/xray_pneumonia.jpeg' | relative_url }}" width="200" height="200">
    <p style="font-size: 0.9em; color: #666;">Pneumonia</p>
  </div>

</div>

<p style="text-align: center; font-size: 0.9em; color: #666; margin-top: 10px;">
  Figure: Example X-ray images of a healthy individual and a pneumonia patient.
</p>


<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
<a href="https://github.com/katwre/ML-projects/blob/main/CNN_and_TransferLearning_Xray/" target="_blank">https://github.com/katwre/ML-projects/blob/main/CNN_and_TransferLearning_Xray/</a>
</p>


<!--  Autoencoder -->
<p class="mytext" id="ae"><span style="color:#505050; font-weight:bold;">Autoencoder for scRNA-seq dimensionality reduction and data imputation</span></p>

<p class="mytext">
I developed a simple autoencoder with a custom loss function for imputing missing values in single-cell RNA-seq data. The approach was inspired by the method proposed by Badsha et al. (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7144625/).
</p>

<div style="text-align: center;">
  <img src="{{ 'img/ae_imputed.png' | relative_url }}" width="400" height="300">
  <p class="mytext" style="text-align: center;font-size: 0.9em; color: #666;">Figure: Imputed scRNA-seq.</p>
</div>


<div style="text-align: center;">
  <img src="{{ 'img/imputed.png' | relative_url }}" width="400" height="250">
  <p class="mytext" style="text-align: center;font-size: 0.9em; color: #666;">Figure: Model's output and the true gene expression values. Non-imputed data (blue): where the model reconstructed known values. Imputed data (orange): where the model predicted missing (masked) values.</p>
</div>


<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
<a href="https://github.com/katwre/ML-projects/tree/main/autoencoder_scRNAseq/" target="_blank">https://github.com/katwre/ML-projects/tree/main/autoencoder_scRNAseq/</a>
</p>


<!--  vae_federated -->
<p class="mytext" id="vae_federated"><span style="color:#505050; font-weight:bold;">Variational autoencoder (VAE) to mitigate batch effects in scRNA-seq using federated learning</span></p>


<p class="mytext">
This project explored a scVI model (variational autoencoder for single-cell data) in a federated setting using the Flower framework (Flower.ai) and the SecAgg+ secure aggregation protocol. For comparison, the same model was also trained in a centralized setting.
</p>

<div style="text-align: center;">
  <img src="{{ 'img/Gene_Expression_UMAP_before_correction.png' | relative_url }}" width="600" height="200">
  <p class="mytext" style="text-align: center;font-size: 0.9em; color: #666;">Figure: Baseline Gene Expression UMAP.</p>
</div>

<div style="text-align: center;">
  <img src="{{ 'img/Gene_Expression_UMAP_after_correction_centralized.png' | relative_url }}" width="600" height="200">
  <p class="mytext" style="text-align: center;font-size: 0.9em; color: #666;">Figure: Centralized scVI Model.</p>
</div>

<div style="text-align: center;">
  <img src="{{ 'img/Gene_Expression_UMAP_after_correction_federated.png' | relative_url }}" width="600" height="200">
  <p class="mytext" style="text-align: center;font-size: 0.9em; color: #666;">Figure: Federated scVI Model.</p>
</div>


<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
<a href="https://github.com/katwre/ML-projects/tree/main/federated_learning_scRNA-seq/" target="_blank">https://github.com/katwre/ML-projects/tree/main/federated_learning_scRNA-seq/</a>
</p>




<!--  deconvolution -->
<p class="mytext" id="deconvolution"><span style="color:#505050; font-weight:bold;">VAE, BERT, semi-supervised NMF and lasso/ridge/elastic net for the cell type deconvolution</span></p>


<p class="mytext">
This project studies cell-free DNA (cfDNA) fragments that circulate in the blood. These fragments originate from many different cell types across the body. When tissues are damaged or diseased, they release more DNA than usual, altering the overall composition of cfDNA in the bloodstream. By identifying which cell types the DNA comes from, we can gain an early view of tissue health and disease signals.

I applied several deconvolution methods to estimate cell type proportions from bulk DNA methylation data. Regression-based approaches (NNLS, Lasso, Ridge, Elastic Net) model methylation profiles as mixtures of reference cell types. In addition, I developed:
<ul class="mytext" style="list-style-type: disc; margin-left: 110px;">
      <li>A variational autoencoder (VAE) that reconstructs CpG profiles while jointly predicting cell type proportions.</li>
      <li>A semi-supervised NMF (ssNMF) that anchors factorization to known reference signatures.</li>
      <li>A lightweight transformer model, treating CpG regions as tokens with embeddings and self-attention to capture genomic dependencies.</li>
</ul>  

<div style="text-align: center;">
  <img src="{{ 'img/deconvlution_bsseq.png' | relative_url }}" width="600" height="200">
  <p class="mytext" style="text-align: center;font-size: 0.9em; color: #666;">Figure: Deconvolution of the DNA methylation signal from blood DNA sequenced using Bisulfite-seq.</p>
</div>
</p>

<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
<a href="https://github.com/katwre/ML-projects/blob/main/VAE_NMF_Transformer_regression_cfDNA/" target="_blank">https://github.com/katwre/ML-projects/blob/main/VAE_NMF_Transformer_regression_cfDNA/</a>
</p>




<!--  LLM -->
<p class="mytext" id="llm"><strong>LLM-based assistant for bioinformatics queries</strong></p>

<p class="mytext">
This project explored an AI-powered assistant that helps researchers ask questions about biology in plain English and automatically turns them into SPARQL queries against public databases:

<ul class="mytext" style="list-style-type: disc; margin-left: 110px;">
  <li>UniProt - proteins, sequences, and annotations</li>
  <li>OMA - orthologs and evolutionary relationships</li>
  <li>Bgee - gene expression across species</li>
</ul>

</p>


<p class="mytext">
The assistant is powered by LLMs (Mistral, Llama via Groq, Ollama) combined with retrieval-augmented generation (RAG) using Qdrant and FastEmbed. You can interact with the assistant either in the terminal/CLI or through a simple chat web app (Chainlit web UI).

Key goals:
<ul class="mytext" style="list-style-type: disc; margin-left: 110px;">
      <li>Allow researchers to query complex biological knowledge bases witha nice web interface.</li>
      <li>Validate and execute queries automatically.</li>
      <li>Provide results summarized in plain language.</li>
</ul>  
</p>

<div style="text-align: center;">
  <img src="{{ 'img/ChainlitwebUI_1.png' | relative_url }}" width="600" height="400">
  <p class="mytext" style="text-align: center;font-size: 0.9em; color: #666;">Figure: A web UI for prompting an LLM of choice (Mistral, Llama via Groq, Ollama).</p>
</div>


<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
<a href="https://github.com/katwre/ML-projects/tree/main/llm-biodata/" target="_blank">https://github.com/katwre/ML-projects/tree/main/llm-biodata/</a>
</p>





<!--  -->
<!-- Computational biology & algorithms (Replica Monte Carlo, de Bruijn graph) -->
<!--  -->

<p class="mytext" id="algorithms"><strong>Computational biology & algorithms</strong></p>


<!-- Protein Folding -->
<p class="mytext" id="rmc"><span style="color:#505050; font-weight:bold;">Protein Folding in the HP Model (Replica Monte Carlo)</span></p>

<p class="mytext">
  Implementation of simulated annealing and replica exchange Monte Carlo algorithm for protein folding in the Hydrophobic Polar (HP) model in Python and NumPy. The HP model simplifies protein folding by using hydrophobic (H) and polar (P) amino acids on a square lattice. Metropolis–Hastings algorithm enables sampling protein configurations based on the Boltzmann distribution.
</p>


<div style="text-align: center;">
  <img src="{{ 'img/HPmodel1.png' | relative_url }}" width="300" height="200">
  <p class="mytext" style="text-align: center;font-size: 0.9em; color: #666;">Figure: HP model protein folding schematic in 2D lattice. Filled, black circles represent hydrophobic residues while unfilled circles represent polar residues. The conformation above yields an optimal energy score in the HP model of -2. The two hydrophobic contacts contributing to the score are between residues 4 and 13 and between residues 5 and 12 (<a href="https://doi.org/10.1186/1471-2105-8-342" target="_blank">Thachuk et al. 2007</a>).</p>
</div>


<p class="mytext" style="text-align: center;font-family: 'Cormorant Garamond', serif;">
<a href="https://github.com/katwre/bioinformatics-projects/tree/master/Molecular_Dynamics" target="_blank">https://github.com/katwre/bioinformatics-projects/tree/master/Molecular_Dynamics</a>
</p>



<!-- Genome Assembly -->
<p class="mytext" id="debrujn"><span style="color:#505050; font-weight:bold;">Genome assembly (de Bruijn graph, Eulerian walk)</span></p>

<p class="mytext">
Implementation of de Bruijn graph-based genome assembly with Eulerian walk to reconstruct DNA sequences from k-mers. Includes short-read assembly principles based on publications by <a href="https://doi.org/10.1038/nbt.2023" target="_blank" rel="noopener">Compeau et al. (2011)</a> and <a href="https://doi.org/10.1073/pnas.171285098" target="_blank" rel="noopener">Pevzner et al. (2001)</a>
</p>

<div style="text-align: center;">
  <img src="{{ 'img/deBruijngraph.png' | relative_url }}" style="max-width: 400px; width: 70%;">
  <p class="mytext" style="text-align: center;font-size: 0.9em; color: #666;">Figure: a schematic example of creating a de Bruijn graph from a DNA sequence containing repeats (Compeau et al. 2011).</p>
</div>


<p class="mytext">
My focus was on modern short-read assembly algorithms construct a de Bruijn graph by representing all k-mer prefixes and suffixes as nodes and then drawing edges that represent k-mers having a particular prefix and suffix. For example, the k-mer edge ATG has prefix AT and suffix TG. Finding an Eulerian cycle allows one to reconstruct the genome by forming an alignment in which each successive k-mer (from successive edges) is shifted by one position. This generates the same cyclic genome sequence without performing the computationally expensive task of finding a Hamiltonian cycle (as shown in the figure below).
</p>


<div style="text-align: center;">
  <img src="{{ 'img/Euleriancycle.png' | relative_url }}" style="max-width: 500px; width: 70%;">
  <p class="mytext" style="text-align: center;font-size: 0.9em; color: #666;">Figure: Two strategies for genome assembly: from Hamiltonian cycles to Eulerian cycles (Pevzner et al. 2001). My focus was on the Eulerian cycle (subfigure d).</p>
</div>


<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
<a href="https://github.com/katwre/bioinformatics-projects/tree/master/genome_assembly" target="_blank">https://github.com/katwre/bioinformatics-projects/tree/master/genome_assembly</a>
</p>

<!-- Evolutionary tree estimation - Felsenstein & NNI -->
<p class="mytext" id="felnni"><span style="color:#505050; font-weight:bold;">Evolutionary tree estimation - Felsenstein & NNI</span></p>

<p class="mytext">
Implementation of the Felsenstein's tree-pruning and the Nearest-Neighbor Interchange (NNI) algorithms. The Felsenstein's tree-pruning is a heuristic algorithm for computing the likelihood of an evolutionary tree from nucleic acid sequence data. It is devoted to searching for an optimal tree structure. NNI is great for rooted binary phylogenetic trees and using Jukes and Cantor substitution model. It is one of the simplest tree-rearrangement methods.
</p>

<div style="text-align: center;">
  <img src="{{ 'img/nni.png' | relative_url }}" style="max-width: 500px; width: 70%;">
  <p class="mytext" style="text-align: center;font-size: 0.9em; color: #666;">Figure: An example of applying an NNI to a subsplit directed acyclic graph (sDAG) <a href="https://almob.biomedcentral.com/articles/10.1186/s13015-025-00273-x" target="_blank">(Jennings-Shaffer et al. 2025)</a>.</p>
</div>

<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
<a href="https://github.com/katwre/bioinformatics-projects/tree/master/comparative_genomics" target="_blank">https://github.com/katwre/bioinformatics-projects/tree/master/comparative_genomics</a>
</p>


<!-- Regulatory DNA discovery - MSA & binomial enrichment -->
<p class="mytext" id="binomial"><span style="color:#505050; font-weight:bold;">Regulatory DNA discovery - MSA & binomial enrichment</span></p>

<p class="mytext">
Bio Motif Ensembl is a Python tool for discovering potential regulatory DNA regions across related mammalian genomes using Ensembl’s public MySQL databases. It retrieves orthologous gene sequences (e.g., human, mouse, rat), aligns their upstream regions, and detects conserved non-coding segments. These conserved blocks are then analyzed with motif discovery algorithms such as MEME and AlignACE, and tested for statistical overrepresentation using a binomial model. The framework integrates comparative genomics, multiple sequence alignment, and motif enrichment to identify functionally significant regulatory elements.
</p>

<div style="text-align: center;">
  <img src="{{ 'img/overreprmotifs.png' | relative_url }}" style="max-width: 500px; width: 70%;">
  <p class="mytext" style="text-align: center;font-size: 0.9em; color: #666;">Figure: It's a similar concept to the approach published by <a href="https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.0020036" target="_blank">MacIsaac et al. 2025</a>.</p>
</div>

<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
<a href="https://github.com/katwre/bioinformatics-projects/tree/master/bio_motif_ensembl" target="_blank">https://github.com/katwre/bioinformatics-projects/tree/master/bio_motif_ensembl</a>
</p>


<hr>


<!--  -->
<!-- Games  -->
<!--  -->

<p class="mytext" id="games"><strong>Games: Sudoku (JavaScript) and Minesweeper (Java)</strong></p>




<!-- Sudoku -->


<p class="mytext" id="sudoku"><span style="color:#505050; font-weight:bold;">Sudoku</span></p>

<p class="mytext">A simple Sudoku game implemented in JavaScript and JQuery. </p>

<div style="text-align: center;">
  <img src="{{ 'img/sudoku.png' | relative_url }}" width="400" height="300">
</div>
<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
<a href="https://github.com/katwre/sudoku" target="_blank">https://github.com/katwre/sudoku</a>



<!-- Minesweeper -->

<p class="mytext" id="minesweeper"><span style="color:#505050; font-weight:bold;">Minesweeper</span></p>

<p class="mytext">A classic Minesweeper game implemented in Java using SWING and AWT libraries.</p>

<div style="text-align: center;">
  <img src="{{ 'img/minesweeper.png' | relative_url }}" width="200" height="230">
</div>
<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
<a href="https://github.com/katwre/Minesweeper" target="_blank">https://github.com/katwre/Minesweeper</a>
</p>

<hr>



<!-- Django Web-Services -->
<p class="mytext" id="django"><strong>Django-Based Web Services</strong></p>
<p class="mytext">
Django-based server for Multiple Sequence Alignment (MSA) visualization - <a href="https://github.com/freesci/MSA-vis-project" target="_blank">https://github.com/freesci/MSA-vis-project</a>

</p>
<p class="mytext">
Mobile application using Django, manifesto app, and localStorage - <a href="https://github.com/katwre/phone_application" target="_blank">https://github.com/katwre/phone_application</a>
</p>

<hr>


<!-- Discover Career Match -->
<p class="mytext" id="pyodine"><strong>Discover Your Career Match (Pyodine)</strong></p>
<p class="mytext">
Interactive tool that matches careers to users based on their personality profile (Big Five personality traits). Runs directly in the browser via Pyodide.
</p>

<div style="text-align: center;">
  <img src="{{ 'img/personalities.png' | relative_url }}" alt="PCA plot of careers based on personality traits" style="max-width: 70%; max-height: 70%; border: 1px solid #ccc; box-shadow: 2px 2px 6px #ddd;">

  <p class="mytext" style="text-align: center;font-size: 0.9em; color: #666;">Figure: PCA plot showing career matches based on personality profile.</p>
</div>
<p class="mytext" style="font-family: 'Cormorant Garamond', serif;">
  <a href="https://github.com/katwre/Personalities" target="_blank">https://github.com/katwre/Personalities</a>
  </p>

