---
layout: page
title: ""
permalink: /projects/

---

<style>

/* Base Typography */
h1, .page-title {
  font-family: 'Cormorant Garamond', serif;
  font-size: 36px;
  font-weight: bold;
  color: #1a1a1a;
  text-align: center;
  margin-bottom: 10px;
}

h2 {
  font-family: 'Cormorant Garamond', serif;
  font-size: 42px;
  color: #1a1a1a;
  text-align: center;
  margin: 60px auto 30px auto;
  padding: 20px;
  position: relative;
}

h2::after {
  content: '';
  display: block;
  width: 80px;
  height: 3px;
  background: linear-gradient(to right, #80002a, #b8003d);
  margin: 15px auto 0;
}

/* Text Styles */
.mytext {
  font-family: 'Inter', sans-serif;
  font-size: 16px;
  color: #2c2c2c;
  line-height: 1.8;
  text-align: justify;
  max-width: 1400px;
  margin: 0 auto 20px auto;
  padding: 0 20px;
}

.mytext a {
  color: #80002a;
  text-decoration: none;
  border-bottom: 1px solid transparent;
  transition: border-bottom 0.3s ease;
}

.mytext a:hover {
  border-bottom: 1px solid #80002a;
}

/* Project Cards */
.project-card {
  max-width: 1500px;
  margin: 40px auto;
  padding: 30px;
  background: #ffffff;
  border-radius: 12px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.08);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.project-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.12);
}

.project-title {
  font-family: 'Cormorant Garamond', serif;
  font-size: 24px;
  font-weight: 600;
  color: #80002a;
  margin-bottom: 15px;
  padding-bottom: 10px;
  border-bottom: 2px solid #f0f0f0;
}

.project-subtitle {
  font-family: 'Inter', sans-serif;
  font-size: 18px;
  font-weight: 600;
  color: #505050;
  margin-top: 25px;
  margin-bottom: 12px;
}

/* Table of Contents */
.toc-wrapper {
  max-width: 1400px;
  margin: 40px auto;
  padding: 30px;
  background: linear-gradient(135deg, #fafafa 0%, #ffffff 100%);
  border-radius: 12px;
  border-left: 4px solid #80002a;
  box-shadow: 0 2px 12px rgba(0, 0, 0, 0.06);
}

.toc-list {
  list-style: none;
  counter-reset: item;
  font-family: 'Georgia', serif;
  font-size: 16px;
  padding-left: 0;
}

.toc-list li {
  display: block;
  margin: 8px 0;
  counter-increment: item;
  line-height: 1.6;
}

.toc-list li:before {
  content: counters(item, ".") " ";
  margin-right: 8px;
  font-weight: 600;
  color: #80002a;
}

.toc-list ol {
  counter-reset: item;
  list-style: none;
  padding-left: 25px;
  margin: 8px 0;
}

.toc-list a {
  text-decoration: none;
  color: #2c2c2c;
  transition: color 0.3s ease;
}

.toc-list a:hover {
  color: #80002a;
}

/* Software Blocks */
.software-block {
  display: flex;
  align-items: center;
  max-width: 1450px;
  margin: 30px auto;
  padding: 25px;
  background: #fafafa;
  border-radius: 10px;
  border: 1px solid #e8e8e8;
  transition: background 0.3s ease;
}

.software-block:hover {
  background: #f5f5f5;
}

.software-logo {
  width: 110px;
  height: auto;
  margin-right: 25px;
  flex-shrink: 0;
}

.software-text {
  font-family: 'Inter', sans-serif;
  font-size: 16px;
  color: #2c2c2c;
  line-height: 1.6;
}

.software-text a {
  color: #80002a;
  text-decoration: none;
  font-weight: 500;
}

.software-text a:hover {
  text-decoration: underline;
}

/* Figure Styling */
figure {
  text-align: center;
  max-width: 1450px;
  margin: 30px auto;
  padding: 20px;
  background: #fafafa;
  border-radius: 10px;
}

figure img {
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

figcaption {
  font-family: 'Georgia', serif;
  font-size: 14px;
  color: #666;
  margin-top: 15px;
  line-height: 1.6;
  font-style: italic;
}

/* Image Gallery */
.image-gallery {
  display: flex;
  justify-content: center;
  gap: 20px;
  flex-wrap: wrap;
  max-width: 1500px;
  margin: 30px auto;
}

.image-gallery-item {
  text-align: center;
  flex: 1;
  min-width: 200px;
}

.image-gallery img {
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease;
}

.image-gallery img:hover {
  transform: scale(1.05);
}

/* Lists */
.mytext ul {
  list-style-type: disc;
  margin-left: 40px;
  line-height: 1.8;
}

.mytext ul li {
  margin: 8px 0;
}

/* Section Dividers */
hr {
  max-width: 1300px;
  margin: 60px auto;
  border: none;
  border-top: 2px solid #e8e8e8;
}

/* Utility Classes */
.emphasize {
  color: #80002a;
  font-weight: 500;
}

.text-center {
  text-align: center;
}

/* Responsive Design */
@media (max-width: 768px) {
  h2 {
    font-size: 32px;
  }
  
  .project-card {
    padding: 20px;
    margin: 30px 15px;
  }
  
  .software-block {
    flex-direction: column;
    text-align: center;
  }
  
  .software-logo {
    margin-right: 0;
    margin-bottom: 15px;
  }
  
  .image-gallery {
    flex-direction: column;
  }
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
        <li><a href="#alzheimer">Multi-omics and AI (Enformer) for an Alzheimer's disease biomarker</a></li>
        <li><a href="#igv">IGV web app feature development</a></li>       
      </ol>
    </li>
    <li>
      <strong><a href="#sideprojects">Projects</a></strong>
      <ol>

    <li><a href="#mldlapi">Machine and deep learning end-to-end projects with APIs</a>
    <ol>
        <li><a href=""> Gene type prediction from DNA sequence using a Transformer encoder - ONNX Runtime inference, FastAPI + BentoML serving, Docker compose, deployed on AWS EKS (Kubernetes)</a></li>
        <li><a href="#debrujn">Predicting Molecular Solubility in Water via a Flask API deployed on AWS Elastic Beanstalk</a></li>
        <li><a href="">Immune cell classifier trained on H&E-stained images using Xception + MLP, exported to TFLite and deployed via Docker and AWS Lambda</a></li>
        <li><a href="">Diffusion-based generative modeling and inpainting of H&E-stained blood cell images, deployed via Streamlit and AWS Batch</a></li>
        </ol> 
    </li>
        <li><a href="#survival">Survival analysis using gene expression & clinical data (Cox models)</a></li>
        <li><a href="#dlomics">Deep learning for xray images and scRNAseq (CNNs, transfer learning, VAE, NMF, BERT)</a></li>
        <li><a href="#gnnspatial">GNN for spatial transcriptomics</a></li>
        <li><a href="#llm">LLM-based assistant for bioinformatics queries</a></li>
        <li><a href="#algorithms">Computational biology & algorithms</a></li>
        <ol>
        <li><a href="#rmc">Protein folding - Monte Carlo</a></li>
        <li><a href="#debrujn">Genome assembly - de Bruijn graph, euler walk</a></li>
        <li><a href="#felnni">Evolutionary tree estimation - Felsenstein & NNI</a></li>
        <li><a href="#binomial">Regulatory DNA discovery - MSA & binomial enrichment</a></li>
        </ol> 
        <li><a href="#games">Games: Sudoku (JavaScript) and Minesweeper (Java)</a></li>
        <li><a href="#django">Django web services (Django-based Multiple Sequence Alignment visualization, Django-based mobile app, Pyodine-based in-browser Python career-matching tool)</a></li>
      </ol>
    </li>
</ol>
</div>




<!--   -->
<!-- Research -->
<!--   -->

<h2 id="research">Research</h2>

<!-- Bias detection and interpretation in genomics experiment -->
<div class="project-card" id="genomics">
  <div class="project-title">Bias interpretation in genomics</div>
  
  <p class="mytext">
    We used machine learning models - elastic net regression and principal component analysis (PCA) - 
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

  <figure>
    <img src="/img/hot.png" alt="HOT regions figure" style="width: 80%; height: auto;">
    <figcaption>
      Figure: Unexpected ChIP-seq signals appear in HOT regions even without the target protein (KO ChIP-seq). 
      The barplot shows how often these regions are detected as bound - 
      HOT regions correspond to the top 1% of genomic regions with the highest protein binding signals (99th percentile).
    </figcaption>
  </figure>

  <p class="mytext">
    <a href="https://doi.org/10.1093/nar/gkv681" target="_blank">
      📄 Publication: Wreczycka K et al, Nucleic Acids Research, 2019
    </a>
  </p>
</div>
  


<!-- cfDNA methylation biomarkers in acute coronary syndrome -->
<div class="project-card" id="cfDNA">
  <div class="project-title">Liquid biopsy epigenetics in disease</div>
  
  <div class="project-subtitle">DNA methylation biomarkers in acute coronary syndrome (blood-derived cfDNA)</div>

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

  <figure>
    <img src="/img/cfndaacs.png" alt="cfDNA ACS figure" style="width: 40%; height: auto;">
    <figcaption>
      Figure: PCA of 254 differentially methylated regions linked to ACS severity using linear models.
    </figcaption>
  </figure>

  <p class="mytext">
    <a href="https://doi.org/10.1093/nargab/lqad061" target="_blank">
    📄 Publication: Rafael R C Cuadrat et al, NAR Genomics and Bioinformatics, 2023
    </a>
  </p>

  <div class="project-subtitle">DNA methylation profiling in neuroblastoma (solid tissues and urine-derived cfDNA)</div>

  <p class="mytext">
    Neuroblastoma is a pediatric cancer ranging from mild to aggressive forms. While genetic changes explain some variability, 
    we showed that DNA methylation plays a key role in its progression. 
    In collaboration with Charité Hospital (Berlin), we analyzed primary tumor tissues and urine cfDNA 
    using bisulfite-seq and RNA-seq, identifying methylation patterns 
    distinguishing high- and low-risk tumors. We also linked MYCN-driven 
    methylation changes to disrupted transcription factor networks, highlighting potential targets for therapies.
  </p>

  <figure>
    <img src="/img/neuroblastoma_clustering.png" alt="Neuroblastoma clustering" style="width: 80%; max-width: 600px;">
    <figcaption>
      Figure: Methylation-based clustering of neuroblastoma patients using differentially methylated CpGs.
    </figcaption>
  </figure>
</div>



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
<div class="project-card" id="target">
  <div class="project-title">Prioritization of therapeutic targets in clinical trials</div>
  
  <div class="project-subtitle">Visualization and survival analysis of biomarkers</div>

  <p class="mytext">
    We developed interactive visualizations, including oncoprints, to highlight key biomarkers in patients with limited treatment options. These visual summaries help uncover genomic alterations and support identifying new therapeutic targets.
  </p>

  <p class="mytext">
    We focused on patients from clinical trial databases facing poor outcomes or lacking effective therapies. Our statistical analyses, including survival analysis, demonstrate the clinical relevance of nominated targets.
  </p>

  <div class="image-gallery">
    <div class="image-gallery-item">
      <img src="{{ '/img/oncoprint_modified.png' | relative_url }}" style="max-width:100%;">
    </div>
    <div class="image-gallery-item">
      <img src="{{ '/img/survival_analysis.png' | relative_url }}" style="max-width:100%;">
    </div>
  </div>
  <p class="mytext text-center" style="font-size: 14px; color: #666;">
    Figure: Example of biomarker visualization and survival analysis.
  </p>

  <div class="project-subtitle" id="mltarget">Machine learning/AI for target identification</div>

  <p class="mytext">
    To prioritize therapeutic targets, we applied <a href="https://cseweb.ucsd.edu/~elkan/posonly.pdf" target="_blank">Positive and Unlabeled (PU) learning</a>, ideal for cases where only confirmed targets are known. PU classifiers helped distinguish potential targets using gene expression, mutations, and therapy annotations.
  </p>
  
  <figure>
    <img src="{{ '/img/PUlearning.png' | relative_url }}" style="max-width:100%;">
    <figcaption>
      Figure: PU learning principle (figure adapted from <a href="https://techblog.ing.pl/blog/podstawy-positive-unlabeled-learning" target="_blank">a blogpost</a>).
    </figcaption>
  </figure>

  <p class="mytext">
    Additionally, we utilized autoencoders to uncover hidden patterns and prioritize key molecular features in an unsupervised way.
  </p>
  
  <figure>
    <img src="{{ 'img/variational-autoencoder.png' | relative_url }}" style="max-width:70%;">
    <figcaption>
      Figure: Schematic of a Variational Autoencoder (figure adapted from <a href="https://avandekleut.github.io/vae/" target="_blank">a blogpost</a>).
    </figcaption>
  </figure>
</div>



<!-- Multiomics for Alzheimers  -->
<div class="project-card" id="alzheimer">

<p class="mytext" id="alzheimer"><strong>Multi-omics and AI (Enformer) for an Alzheimer's disease biomarker</strong></p>


<p class="mytext">

In this project, I investigated glial-to-neuron reprogramming through activation of a specific transcription factor (TF) in Alzheimer’s disease.

I integrated multi-omics data - including RNA-seq, ATAC-seq, and H3K4me2/H3K27me3 ChIP-seq - to identify differentially expressed genes and gene pathways (GO, GSEA), their association with Alzheimer’s disease risk variants (GWAS), regulatory enhancers, DNA motifs and TF binding sites linked to neuronal differentiation.

Large-scale analyses were executed via <a href="https://www.nextflow.io/" target="_blank">Nextflow</a> pipelines on Kubernetes and AWS, ensuring scalable and reproducible processing of NGS datasets.
</p>


  <figure>
    <img src="{{ 'img/alzheimers_DL/rnaseq.png' | relative_url }}" style="width: 70%; height: auto;">
    <figcaption>Figure: Example RNA-seq analysis.</figcaption>
  </figure>

  <figure>
    <img src="{{ 'img/alzheimers_DL/motifactivity.png' | relative_url }}" style="width: 70%; height: auto;">
    <figcaption>Figure: Example DNA motif activity in enhancers defined by ATAC-seq, H3K4me2 and H3K27me3 peaks.</figcaption>
  </figure>

  <figure>
    <img src="{{ 'img/alzheimers_DL/chipseqpeaks.png' | relative_url }}" style="width: 70%; height: auto;">
    <figcaption>Figure: Example ChIP-seq peaks around the target TF gene in the IGV browser.</figcaption>
  </figure>

<p class="mytext">
Using <a href="https://www.nature.com/articles/s41592-021-01252-x/" target="_blank">DeepMind’s Enformer model by Avsec et al.</a>, I mapped the regulatory landscape around the target TF to uncover and confirm DNA regions predicted to most strongly influence its expression in neurons and glia. Enformer predicts regulatory activity directly from DNA sequence and uses gradient-based attribution to reveal regions with the strongest impact on gene expression. I analyzed a ~400 kb region around the transcription factor, applying cell-type–specific masks and signal smoothing to identify candidate enhancers.
</p>


<div style="text-align: center;">

  <div style="margin-bottom: 30px;">
    <img src="{{ 'img/alzheimers_DL/enformer.png' | relative_url }}" 
         style="max-width: 50%; height: auto; border-radius: 8px;">
    <div style="font-size: 14px; color: #555;">
      Figure: Enformer’s architecture by 
      <a href="https://www.nature.com/articles/s41592-021-01252-x/" target="_blank">Avsec et al.</a> copied from <a href="https://deepmind.google/discover/blog/predicting-gene-expression-with-ai/" target="_blank">the blog post</a>.
    </div>
  </div>

  <div style="margin-bottom: 30px;">
    <img src="{{ 'img/alzheimers_DL/enformer_output.png' | relative_url }}" 
         style="max-width: 70%; height: auto; border-radius: 8px;">
    <div style="font-size: 14px; color: #555;">
      Figure: Selected tracks corresponding to neurons or glia with Enformer's scores.
    </div>
  </div>

  <div>
    <img src="{{ 'img/alzheimers_DL/enformer_output_enhancers.png' | relative_url }}" 
         style="max-width: 70%; height: auto; border-radius: 8px;">
    <div style="font-size: 14px; color: #555;">
      Figure: Selected Enformer's score peaks as potiential enhancers and highlighted regions of interest.
    </div>
  </div>

</div>
</div>

<br>


<!-- Web app feature development  -->
<div class="project-card" id="igv">
  <div class="project-title">IGV web app feature development</div>

  <p class="mytext">
    I contributed to enhancing the 
    <a href="https://igv.org/app/" target="_blank">IGV web application</a>, 
    an interactive tool for visual exploration of genomic data 
    (<a href="https://github.com/igvteam/igv-webapp" target="_blank">source code</a>).
    Built with JavaScript and Python, this tool allows visualization of both public and in-house datasets.
  </p>
  
  <ul class="mytext">
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
  
  <figure>
    <img src="{{ 'img/igv_original.png' | relative_url }}" style="max-width: 70%; height: auto;">
    <figcaption>Figure: Example IGV web app view showing genomic data tracks.</figcaption>
  </figure>
</div>




<!--   -->
<!-- Side projects -->
<!--   -->


<h2 id="sideprojects">Projects</h2>


<!-- ML/DL with APIs  -->
<div class="project-card" id="mldlapi">
  <div class="project-title">Machine and deep learning end-to-end projects with APIs</div>

  <div class="project-subtitle">Gene type prediction from DNA sequence using a Transformer encoder - ONNX Runtime inference, FastAPI + BentoML serving, Docker compose, deployed on AWS EKS (Kubernetes)</div>
  
  <p class="mytext">
    The aim of this project was to predict gene type directly from a raw DNA sequence using classical machine learning models, convolutional neural networks, and a custom nucleotide-level Transformer, while also exploring practical deployment of machine learning services with Docker compose, Kubernetes (locally with Kind) and cloud infrastructure (AWS Kubernetes EKS)
  </p>

  <figure>
    <img src="{{ 'img/sequence_transformer.png' | relative_url }}" style="width: 60%; max-width: 300px;">
    <figcaption>Figure. An example of a gene and its nucleotide sequence.</figcaption>
  </figure>

    <p class="mytext text-center">
    <a href="https://github.com/katwre/Genetype-classifier-api" target="_blank">🔗 GitHub Repository</a>
  </p>

  <div class="project-subtitle">Predicting Molecular Solubility in Water via a Flask API deployed on AWS Elastic Beanstalk</div>
  
  <p class="mytext">
    The goal of this project was simple: Given a set of molecular descriptors, predict whether a compound will dissolve in water. We provide the model with numeric features that describe the molecule (size, polarity, solvation energy, charge distribution, etc.) and ask: "Will this molecule dissolve, or will it stay stubbornly solid?". I experimented with several regression models — Partial Least Squares (baseline linear model), Elastic Net (linear model with feature selection), Random Forest, and XGBoost (gradient-boosted trees) - to predict whether a molecule will dissolve in water based on its descriptors.
  </p>

  <figure>
    <img src="{{ 'img/solubility.png' | relative_url }}" style="width: 60%; max-width: 400px;">
    <figcaption>Figure. Conceptual view of solubility prediction.</figcaption>
  </figure>

  
  <p class="mytext text-center">
    <a href="https://github.com/katwre/Solubility-api" target="_blank">🔗 GitHub Repository</a>
  </p>


  <div class="project-subtitle">Immune cell classifier using Xception + MLP deployed via Docker and AWS Lambda</div>
  
  <p class="mytext">
    The aim of this project was to evaluate transfer learning-based convolutional neural networks for classifying immune cell types from H&E-stained blood microscopy images. I applied transfer learning with a pretrained Xception model as a fixed feature extractor and trained a small custom MLP classification head on top of it. I additionally extracted Xception embeddings and trained classical machine learning models such as logistic regression and XGBoost to provide an interpretable baseline. Hyperparameters such as learning rate and dropout rate were tuned, and the model using the MLP head achieved strong accuracy on the test set.
  </p>

  <figure>
    <img src="{{ 'img/immunecells.png' | relative_url }}" style="width: 60%; max-width: 400px;">
    <figcaption>Figure. Examples of blood cell types: an erythroblast, a monocyte and a platelet. </figcaption>
  </figure>

   <p class="mytext text-center">
    <a href="https://github.com/katwre/Immune-cell-classifier-api" target="_blank">🔗 GitHub Repository</a>
  </p>


  <div class="project-subtitle">Diffusion-based generative modeling and inpainting of H&E-stained blood cell images, deployed via Streamlit and AWS Batch</div>
  
  <p class="mytext">
    The aim of this project was to explore the ability of diffusion models to generate missing regions in images. It restores corrupted areas in H&E cell images using a compact diffusion model and a simple Streamlit UI.
  </p>

  <figure>
    <img src="{{ 'img/diffusion_immune.png' | relative_url }}" style="width: 60%; max-width: 400px;">
    <figcaption>Figure. Diffusion-based inpainting results. The model reconstructs masked regions while preserving the observed context.</figcaption>
  </figure>

  <p class="mytext text-center">
    <a href="https://github.com/katwre/Diffusion-models-for-cell-images-api" target="_blank">🔗 GitHub Repository</a>
  </p>

</div>


<!-- survival  -->
<div class="project-card" id="survival">
  <div class="project-title">Survival analysis using gene expression & clinical data (Cox models)</div>

  <p class="mytext">
    I developed several survival models to predict the risk of mortality or relapse in newly diagnosed multiple myeloma patients, using baseline clinical and/or gene expression data. The workflow involved RNA-seq preprocessing, unsupervised exploratory analysis (PCA, clustering), and multiple survival modeling strategies - Cox regression, random survival forests, LASSO-based feature selection, and pathway-informed models - evaluated using the C-index.
  </p>

  <div class="image-gallery">
    <div class="image-gallery-item">
      <img src="{{ 'img/survival_classification.png' | relative_url }}" style="width: 100%; max-width: 550px;">
    </div>
    <div class="image-gallery-item">
      <img src="{{ 'img/surival_probability.png' | relative_url }}" style="width: 100%; max-width: 300px;">
    </div>
  </div>
  <p class="mytext text-center" style="font-size: 14px; color: #666;">
    Figure: C-index comparison of multiple survival models (left) and Kaplan–Meier plot of the best performing model (right).
  </p>

  <p class="mytext text-center">
    <a href="https://github.com/katwre/survival_analysis/tree/main/" target="_blank">🔗 GitHub Repository</a>
  </p>
</div>





<!--   -->
<!-- DL in omics  -->
<!--   -->

<div class="project-card" id="dlomics">

  <div class="project-title">Deep learning for xray images and omics (CNNs, transfer learning, VAE, NMF, BERT, GNN)</div>

  <div class="project-subtitle" id="cnn">CNNs and transfer learning for image classification tasks based on chest X-rays</div>

  <p class="mytext">
    I applied convolutional neural networks (CNNs) to classify chest X-ray images using both 224×224 and 64×64 pixel inputs, aiming to explore whether lightweight models can retain sufficient diagnostic power for image-based classification tasks. In addition to training a baseline CNN from scratch, I employed transfer learning with pretrained convolutional backbones such as ResNet to evaluate whether pretrained models could further enhance classification performance on chest X-ray images.
  </p>

  <div class="image-gallery">
    <div class="image-gallery-item">
      <img src="{{ 'img/xray.jpeg' | relative_url }}" width="200" height="200">
      <p style="font-size: 0.9em; color: #666; margin-top: 8px;">Healthy</p>
    </div>
    <div class="image-gallery-item">
      <img src="{{ 'img/xray_pneumonia.jpeg' | relative_url }}" width="200" height="200">
      <p style="font-size: 0.9em; color: #666; margin-top: 8px;">Pneumonia</p>
    </div>
  </div>
  <p class="mytext text-center" style="font-size: 14px; color: #666;">
    Figure: Example X-ray images of a healthy individual and a pneumonia patient.
  </p>

  <p class="mytext text-center">
    <a href="https://github.com/katwre/ML-projects/blob/main/CNN_and_TransferLearning_Xray/" target="_blank">🔗 GitHub Repository</a>
  </p>
<!--  </div> -->


<!--  <div class="project-card" id="ae"> -->

  <div class="project-subtitle" id="ae">Autoencoder for scRNA-seq dimensionality reduction and data imputation</div>

  <p class="mytext">
    I developed a simple autoencoder with a custom loss function for imputing missing values in single-cell RNA-seq data. The approach was inspired by the method proposed by Badsha et al. (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7144625/).
  </p>

  <figure>
    <img src="{{ 'img/ae_imputed.png' | relative_url }}" style="width: 60%; max-width: 400px;">
    <figcaption>Figure: Imputed scRNA-seq.</figcaption>
  </figure>

  <figure>
    <img src="{{ 'img/imputed.png' | relative_url }}" style="width: 60%; max-width: 400px;">
    <figcaption>Figure: Model's output and the true gene expression values. Non-imputed data (blue): where the model reconstructed known values. Imputed data (orange): where the model predicted missing (masked) values.</figcaption>
  </figure>

  <p class="mytext text-center">
    <a href="https://github.com/katwre/ML-projects/tree/main/autoencoder_scRNAseq/" target="_blank">🔗 GitHub Repository</a>
  </p>


  <div class="project-subtitle" id="vae_federated">Variational autoencoder (VAE) to mitigate batch effects in scRNA-seq using federated learning</div>

  <p class="mytext">
    This project explored a scVI model (variational autoencoder for single-cell data) in a federated setting using the Flower framework (Flower.ai) and the SecAgg+ secure aggregation protocol. For comparison, the same model was also trained in a centralized setting.
  </p>

  <figure>
    <img src="{{ 'img/Gene_Expression_UMAP_before_correction.png' | relative_url }}" style="width: 80%; max-width: 600px;">
    <figcaption>Figure: Baseline Gene Expression UMAP.</figcaption>
  </figure>

  <figure>
    <img src="{{ 'img/Gene_Expression_UMAP_after_correction_centralized.png' | relative_url }}" style="width: 80%; max-width: 600px;">
    <figcaption>Figure: Centralized scVI Model.</figcaption>
  </figure>

  <figure>
    <img src="{{ 'img/Gene_Expression_UMAP_after_correction_federated.png' | relative_url }}" style="width: 80%; max-width: 600px;">
    <figcaption>Figure: Federated scVI Model.</figcaption>
  </figure>

  <p class="mytext text-center">
    <a href="https://github.com/katwre/ML-projects/tree/main/federated_learning_scRNA-seq/" target="_blank">🔗 GitHub Repository</a>
  </p>

<!-- </div> -->


<!--  <div class="project-card" id="deconvolution"> -->


  <div class="project-subtitle" id="deconvolution">VAE, BERT, semi-supervised NMF and lasso/ridge/elastic net for cell type deconvolution</div>

  <p class="mytext">
    This project studies cell-free DNA (cfDNA) fragments that circulate in the blood. These fragments originate from many different cell types across the body. When tissues are damaged or diseased, they release more DNA than usual, altering the overall composition of cfDNA in the bloodstream. By identifying which cell types the DNA comes from, we can gain an early view of tissue health and disease signals.
  </p>

  <p class="mytext">
    I applied several deconvolution methods to estimate cell type proportions from bulk DNA methylation data. Regression-based approaches (NNLS, Lasso, Ridge, Elastic Net) model methylation profiles as mixtures of reference cell types. In addition, I developed:
  </p>
  
  <ul class="mytext">
    <li>A variational autoencoder (VAE) that reconstructs CpG profiles while jointly predicting cell type proportions.</li>
    <li>A semi-supervised NMF (ssNMF) that anchors factorization to known reference signatures.</li>
    <li>A lightweight transformer model, treating CpG regions as tokens with embeddings and self-attention to capture genomic dependencies.</li>
  </ul>

  <figure>
    <img src="{{ 'img/deconvlution_bsseq.png' | relative_url }}" style="width: 80%; max-width: 600px;">
    <figcaption>Figure: Deconvolution of the DNA methylation signal from blood DNA sequenced using Bisulfite-seq.</figcaption>
  </figure>

  <p class="mytext text-center">
    <a href="https://github.com/katwre/ML-projects/blob/main/VAE_NMF_Transformer_regression_cfDNA/" target="_blank">🔗 GitHub Repository</a>
  </p>
</div>


<div class="project-card" id="gnnspatial">

  <div class="project-subtitle" id="gnnspatial">GNN for spatial transcriptomics</div>

  <p class="mytext">
    This project's aim was to demonstrate how GNNs can capture spatially coherent patterns in gene expression and to compare these learned embeddings to traditional PCA and k-means-based clustering.
  </p>

  <p class="mytext">
    Spatial transcriptomics captures gene expression while preserving tissue architecture, enabling the study of cellular organization and microenvironments. However, identifying coherent spatial domains, regions of similar expression patterns and spatial context, remains challenging.
  </p>

  <p class="mytext">
    Graph Neural Networks (GNNs) are great for this type of data because they can model both gene expression features and spatial neighborhood relationships. In this project, I implemented a mini Graph Autoencoder (GAE) from scratch in PyTorch to learn unsupervised spatial embeddings of tissue spots from a toy Visium H&E dataset provided by Squidpy (a 10x Genomics Visium H&E mouse brain section (~2,700 spots, ~33k genes)).
  </p>

  <div class="image-gallery">
    <div class="image-gallery-item">
      <img src="{{ 'img/gnn_spatial_baseline.png' | relative_url }}" width="300" height="300">
      <p class="mytext" style="font-size: 0.9em; color: #666; margin-top: 8px;">Figure: Baseline PCA + KMeans.</p>
    </div>
    <div class="image-gallery-item">
      <img src="{{ 'img/gnn_spatial.png' | relative_url }}" width="300" height="300">
      <p class="mytext" style="font-size: 0.9em; color: #666; margin-top: 8px;">Figure: GNN-based clustering.</p>
    </div>
  </div>

  <p class="mytext text-center">
    <a href="https://github.com/katwre/ML-projects/tree/main/GNN_spatialomics" target="_blank">🔗 GitHub Repository</a>
  </p>
</div>



<!--  LLM -->
<div class="project-card" id="llm">
  <div class="project-title">LLM-based assistant for bioinformatics queries</div>

  <p class="mytext">
    This project explored an AI-powered assistant that helps researchers ask questions about biology in plain English and automatically turns them into SPARQL queries against public databases:
  </p>

  <ul class="mytext">
    <li>UniProt - proteins, sequences, and annotations</li>
    <li>OMA - orthologs and evolutionary relationships</li>
    <li>Bgee - gene expression across species</li>
  </ul>

  <p class="mytext">
    The assistant is powered by LLMs (Mistral, Llama via Groq, Ollama) combined with retrieval-augmented generation (RAG) using Qdrant and FastEmbed. You can interact with the assistant either in the terminal/CLI or through a simple chat web app (Chainlit web UI).
  </p>

  <p class="mytext">Key goals:</p>
  <ul class="mytext">
    <li>Allow researchers to query complex biological knowledge bases with a nice web interface.</li>
    <li>Validate and execute queries automatically.</li>
    <li>Provide results summarized in plain language.</li>
  </ul>

  <figure>
    <img src="{{ 'img/ChainlitwebUI_1.png' | relative_url }}" style="width: 80%; max-width: 600px;">
    <figcaption>Figure: A web UI for prompting an LLM of choice (Mistral, Llama via Groq, Ollama).</figcaption>
  </figure>

  <p class="mytext text-center">
    <a href="https://github.com/katwre/ML-projects/tree/main/llm-biodata/" target="_blank">🔗 GitHub Repository</a>
  </p>
</div>





<!--  -->
<!-- Computational biology & algorithms (Replica Monte Carlo, de Bruijn graph) -->
<!--  -->

<div class="project-card" id="algorithms">
  <div class="project-title">Computational biology & algorithms</div>

  <div class="project-subtitle" id="rmc">Protein Folding in the HP Model (Replica Monte Carlo)</div>

  <p class="mytext">
    Implementation of simulated annealing and replica exchange Monte Carlo algorithm for protein folding in the Hydrophobic Polar (HP) model in Python and NumPy. The HP model simplifies protein folding by using hydrophobic (H) and polar (P) amino acids on a square lattice. Metropolis–Hastings algorithm enables sampling protein configurations based on the Boltzmann distribution.
  </p>

  <figure>
    <img src="{{ 'img/HPmodel1.png' | relative_url }}" style="width: 50%; max-width: 300px;">
    <figcaption>Figure: HP model protein folding schematic in 2D lattice. Filled, black circles represent hydrophobic residues while unfilled circles represent polar residues. The conformation above yields an optimal energy score in the HP model of -2. The two hydrophobic contacts contributing to the score are between residues 4 and 13 and between residues 5 and 12 (<a href="https://doi.org/10.1186/1471-2105-8-342" target="_blank">Thachuk et al. 2007</a>).</figcaption>
  </figure>

  <p class="mytext text-center">
    <a href="https://github.com/katwre/bioinformatics-projects/tree/master/Molecular_Dynamics" target="_blank">🔗 GitHub Repository</a>
  </p>



  <div class="project-subtitle" id="debrujn">Genome assembly (de Bruijn graph, Eulerian walk)</div>

  <p class="mytext">
    Implementation of de Bruijn graph-based genome assembly with Eulerian walk to reconstruct DNA sequences from k-mers. Includes short-read assembly principles based on publications by <a href="https://doi.org/10.1038/nbt.2023" target="_blank" rel="noopener">Compeau et al. (2011)</a> and <a href="https://doi.org/10.1073/pnas.171285098" target="_blank" rel="noopener">Pevzner et al. (2001)</a>
  </p>

  <figure>
    <img src="{{ 'img/deBruijngraph.png' | relative_url }}" style="max-width: 500px; width: 70%;">
    <figcaption>Figure: a schematic example of creating a de Bruijn graph from a DNA sequence containing repeats (Compeau et al. 2011).</figcaption>
  </figure>

  <p class="mytext">
    My focus was on modern short-read assembly algorithms construct a de Bruijn graph by representing all k-mer prefixes and suffixes as nodes and then drawing edges that represent k-mers having a particular prefix and suffix. For example, the k-mer edge ATG has prefix AT and suffix TG. Finding an Eulerian cycle allows one to reconstruct the genome by forming an alignment in which each successive k-mer (from successive edges) is shifted by one position. This generates the same cyclic genome sequence without performing the computationally expensive task of finding a Hamiltonian cycle (as shown in the figure below).
  </p>

  <figure>
    <img src="{{ 'img/Euleriancycle.png' | relative_url }}" style="max-width: 550px; width: 75%;">
    <figcaption>Figure: Two strategies for genome assembly: from Hamiltonian cycles to Eulerian cycles (Pevzner et al. 2001). My focus was on the Eulerian cycle (subfigure d).</figcaption>
  </figure>

  <p class="mytext text-center">
    <a href="https://github.com/katwre/bioinformatics-projects/tree/master/genome_assembly" target="_blank">🔗 GitHub Repository</a>
  </p>

  <div class="project-subtitle" id="felnni">Evolutionary tree estimation - Felsenstein & NNI</div>

  <p class="mytext">
    Implementation of the Felsenstein's tree-pruning and the Nearest-Neighbor Interchange (NNI) algorithms. The Felsenstein's tree-pruning is a heuristic algorithm for computing the likelihood of an evolutionary tree from nucleic acid sequence data. It is devoted to searching for an optimal tree structure. NNI is great for rooted binary phylogenetic trees and using Jukes and Cantor substitution model. It is one of the simplest tree-rearrangement methods.
  </p>

  <figure>
    <img src="{{ 'img/nni.png' | relative_url }}" style="max-width: 550px; width: 75%;">
    <figcaption>Figure: An example of applying an NNI to a subsplit directed acyclic graph (sDAG) <a href="https://almob.biomedcentral.com/articles/10.1186/s13015-025-00273-x" target="_blank">(Jennings-Shaffer et al. 2025)</a>.</figcaption>
  </figure>

  <p class="mytext text-center">
    <a href="https://github.com/katwre/bioinformatics-projects/tree/master/comparative_genomics" target="_blank">🔗 GitHub Repository</a>
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

  <p class="mytext text-center">
    <a href="https://github.com/katwre/bioinformatics-projects/tree/master/bio_motif_ensembl" target="_blank">🔗 GitHub Repository</a>
  </p>



<hr>

<!--  -->
<!-- Games  -->
<!--  -->

<div class="project-card" id="games">
  <div class="project-title">Games: Sudoku (JavaScript) and Minesweeper (Java)</div>

  <div class="project-subtitle" id="sudoku">Sudoku</div>

  <p class="mytext">A simple Sudoku game implemented in JavaScript and JQuery.</p>

  <figure>
    <img src="{{ 'img/sudoku.png' | relative_url }}" style="width: 70%; max-width: 400px;">
  </figure>
  
  <p class="mytext text-center">
    <a href="https://github.com/katwre/sudoku" target="_blank">🔗 GitHub Repository</a>
  </p>

  <div class="project-subtitle" id="minesweeper">Minesweeper</div>

  <p class="mytext">A classic Minesweeper game implemented in Java using SWING and AWT libraries.</p>

  <figure>
    <img src="{{ 'img/minesweeper.png' | relative_url }}" style="width: 50%; max-width: 200px;">
  </figure>
  
  <p class="mytext text-center">
    <a href="https://github.com/katwre/Minesweeper" target="_blank">🔗 GitHub Repository</a>
  </p>
</div>

<hr>

<!-- Django Web-Services -->
<div class="project-card" id="django">
  <div class="project-title">Django-Based Web Services</div>
  
  <p class="mytext">
    Django-based server for Multiple Sequence Alignment (MSA) visualization - 
    <a href="https://github.com/freesci/MSA-vis-project" target="_blank">🔗 GitHub Repository</a>
  </p>
  
  <p class="mytext">
    Mobile application using Django, manifesto app, and localStorage - 
    <a href="https://github.com/katwre/phone_application" target="_blank">🔗 GitHub Repository</a>
  </p>


<!-- Discover Career Match -->
  <div class="project-title">Discover Your Career Match (Pyodine)</div>
  
  <p class="mytext">
    Interactive tool that matches careers to users based on their personality profile (Big Five personality traits). Runs directly in the browser via Pyodide.
  </p>

  <figure>
    <img src="{{ 'img/personalities.png' | relative_url }}" alt="PCA plot of careers based on personality traits" style="max-width: 75%; height: auto;">
    <figcaption>Figure: PCA plot showing career matches based on personality profile.</figcaption>
  </figure>
  
  <p class="mytext text-center">
    <a href="https://github.com/katwre/Personalities" target="_blank">🔗 GitHub Repository</a>
  </p>
</div>

