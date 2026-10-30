---
title: "NeuralPathways Lab - Prospective students"
layout: page
sitemap: true
permalink: /prospective-students/
---

<style>
.ps-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  margin-bottom: 30px;
}
.ps-card {
  background: #fff;
  border: 1px solid #e0e0e0;
  border-left: 4px solid #337ab7;
  border-radius: 4px;
  padding: 22px 24px;
  flex: 1 1 calc(50% - 20px);
  min-width: 280px;
  box-sizing: border-box;
}
.ps-card h4 {
  margin: 0 0 10px;
  font-weight: 600;
  color: #222;
}
.ps-card ul {
  color: #555;
  font-size: 14px;
  line-height: 1.6;
  margin: 0;
  padding-left: 18px;
}
.ps-project {
  background: #f9f9f9;
  border: 1px solid #e0e0e0;
  border-top: 4px solid #337ab7;
  border-radius: 4px;
  padding: 26px 28px;
  margin: 10px 0 30px;
  text-align: justify;
}
.ps-project h3 {
  margin-top: 0;
}
.ps-project h4 {
  margin-top: 22px;
  font-weight: 600;
}
.ps-status {
  display: inline-block;
  background: #337ab7;
  color: #fff;
  font-size: 13px;
  font-weight: 600;
  padding: 3px 10px;
  border-radius: 3px;
  margin-bottom: 12px;
}
.ps-meta {
  color: #555;
  font-size: 14px;
}
.ps-refs {
  font-size: 13px;
  color: #555;
  line-height: 1.5;
}
</style>

<div markdown="0" style="text-align: justify; margin: 45px 0 30px;">
<p>I am building a computational group at the <a href="https://www.sheffield.ac.uk/sitran">Sheffield Institute for Translational Neuroscience (SITraN)</a>, University of Sheffield, supported by an <a href="https://www.mndassociation.org/research">MND Association</a> Non-Clinical Junior Fellowship and working closely with the Cooper-Knock lab at SITraN and the <a href="https://snyderlab.stanford.edu">Snyder Lab</a> at Stanford. We use single-cell multiomics, spatial transcriptomics and network science to find the genes behind cell-type-specific changes in ALS/MND.</p>
<p>I welcome enquiries from prospective PhD students, and from MSc and summer students looking for a computational project. Below is a PhD project I would like to supervise.</p>
</div>

<div markdown="0" class="ps-grid">

<div class="ps-card">
<h4>Who I am looking for</h4>
<ul>
<li>A degree in biology, biomedical science, bioinformatics, physics, mathematics, computer science or a related subject.</li>
<li>Some programming in Python or R, or a clear plan to learn it quickly.</li>
<li>Curiosity about how cells go wrong in neurodegeneration. No wet-lab experience is needed.</li>
</ul>
</div>

<div class="ps-card">
<h4>What you will learn</h4>
<ul>
<li>Single-cell and spatial genomics with the scverse tools, and statistics for donor-level study designs.</li>
<li>Gene regulatory network inference, network science and high-performance computing.</li>
<li>How to turn large human datasets into testable biology, alongside ALS clinicians, geneticists and wet-lab scientists at SITraN, with collaborators at Stanford and the Federal University of Rio de Janeiro.</li>
</ul>
</div>

</div>

<div markdown="0" class="ps-project">

<span class="ps-status">PhD project proposal</span>

<h3>Understanding oligodendrocyte dysfunction in ALS through gene regulatory network modelling</h3>

<p class="ps-meta"><strong>Supervisors:</strong> Dr Rodrigo Kazu Siqueira and Prof Johnathan Cooper-Knock, SITraN, University of Sheffield<br>
<strong>Close collaborator:</strong> Manu Saraswat, German Cancer Research Center (DKFZ), Heidelberg, developer of <a href="https://github.com/bioFAM/scDoRI">scDoRI</a><br>
<strong>Funding:</strong> this is a proposed project, not yet a funded position. It is open to self-funded students and to candidates applying for competitive studentships or government scholarships, and I will help strong applicants prepare their funding application.</p>

<h4>Background</h4>
<p>ALS is usually described as a disease of motor neurons, but the cells around them change too. Oligodendrocytes wrap axons in myelin and feed them metabolically. In ALS models they degenerate early and are replaced by new cells that fail to mature (Kang et al., 2013), and removing TDP-43 from mature oligodendrocytes is enough to cause motor problems in mice (Heo et al., 2022). In people with ALS, oligodendrocyte gene expression falls in the spinal cord (Humphrey et al., 2023), while single-nucleus data from the motor cortex show their own oligodendrocyte changes (Pineda et al., 2024). We still do not know which transcription factors and gene programmes drive oligodendrocytes into these disease states, or whether the same programmes act in the cortex and the cord. Profiling RNA and chromatin together in single nuclei now lets us rebuild the gene regulatory network of each cell type and ask these questions directly.</p>

<h4>Aims</h4>
<ol>
<li><strong>Map oligodendrocyte regulatory programmes in ALS.</strong> Using our single-nucleus multiome atlas of ALS motor cortex from 70 donors, infer gene regulatory network topics for the oligodendrocyte lineage with scDoRI, working closely with its developer, Manu Saraswat. Compare sporadic and C9orf72 ALS with controls, and classify transcription factors as activators or repressors of each programme.</li>
<li><strong>Find the genes that steer the disease programmes.</strong> Apply network controllability (minimum dominating sets) and centrality measures to the programmes that shift in ALS. Test how stable the candidate controller genes are across donors and across equally small solutions, and rank them against ALS genetics.</li>
<li><strong>Locate them in human tissue.</strong> Test the leading programmes and genes in our spatial transcriptomics data. Relate oligodendrocyte states to TDP-43 pathology in nearby motor neurons in ALS spinal cord (10x Xenium), and compare motor cortex with spinal cord from the same donors (10x Atera).</li>
</ol>

<h4>Methods</h4>
<p>Python and R, scanpy and SnapATAC2, pseudobulk DESeq2, mixed-effects models with donor as a random effect, scDoRI, motif and footprinting analysis, integer linear programming for network control, spatial statistics, and SLURM-based computing. All code will be reproducible and shared openly.</p>

<h4>Timeline</h4>
<ul>
<li><strong>Year 1:</strong> training, quality control, oligodendrocyte regulatory topics and the case-control comparison (Aim 1), and a literature review.</li>
<li><strong>Year 2:</strong> controller genes, robustness and genetic prioritisation (Aim 2), and a first manuscript.</li>
<li><strong>Year 3:</strong> spatial validation in spinal cord and motor cortex (Aim 3), and a second manuscript.</li>
<li><strong>Final months:</strong> thesis writing.</li>
</ul>

<h4>Expected outcomes</h4>
<p>A ranked, reproducible set of oligodendrocyte regulatory programmes and candidate controller genes in ALS, placed in human tissue, with the strongest candidates handed to wet-lab colleagues at SITraN for testing.</p>

<h4>Key references</h4>
<p class="ps-refs">
Kang SH et al. (2013) Degeneration and impaired regeneration of gray matter oligodendrocytes in amyotrophic lateral sclerosis. <i>Nature Neuroscience</i> 16:571-579.<br>
Heo D et al. (2022) Stage-specific control of oligodendrocyte survival and morphogenesis by TDP-43. <i>eLife</i> 11:e75230.<br>
Humphrey J et al. (2023) Integrative transcriptomic analysis of the amyotrophic lateral sclerosis spinal cord implicates glial activation and suggests new risk genes. <i>Nature Neuroscience</i> 26:150-162.<br>
Pineda SS et al. (2024) Single-cell dissection of the human motor and prefrontal cortices in ALS and FTLD. <i>Cell</i> 187:1971-1989.<br>
Saraswat M et al. (2025) Decoding plasticity regulators and transition trajectories in glioblastoma with single-cell multiomics. <i>bioRxiv</i>.
</p>

</div>

<div markdown="0" style="text-align: justify; margin-bottom: 40px;">
<h3>How to get in touch</h3>
<p>Email me at <a href="mailto:r.siqueiradesouza@sheffield.ac.uk">r.siqueiradesouza@sheffield.ac.uk</a> with your CV, your academic transcripts, a one-page statement on why this project interests you and what you would bring to it, and the funding route you plan to use. I am also happy to discuss other project ideas in single-cell and spatial genomics of ALS, or network science applied to biology.</p>
</div>
