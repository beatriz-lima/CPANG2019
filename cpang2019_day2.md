---


---

<h2 id="construct-a-pan-genome">Construct a pan-genome</h2>
<p>There are two ways to construct it: via vg or seqwish. We constructed a pan-genome representation of the five reference genomes.</p>
<h2 id="align-the-data-from-short-reads">Align the data from short reads</h2>
<p>The idea is to align the reads from the Illumina sequencing into both of the graphs and then compare the performance of the graph constructed using vg map vs seqwish by extracting the mapping scores or the identity scores.<br>
The next idea is to compare the performance between using a pan-genome graph vs a linear reference using BWA by mapping the same reads. We found that the pan-genome graph is a better reference than the linear one.<br>
<img src="https://user-images.githubusercontent.com/43668147/64633796-ce1c8500-d3f3-11e9-9a29-9e9c9a86499d.png" alt="image"></p>
<h2 id="output-analysis">Output analysis</h2>
<p>We used vg pack to get the nodes coverage along the graph, then draw the corresponding plot.</p>
<p><img src="https://user-images.githubusercontent.com/43668147/64630741-a4605f80-d3ed-11e9-904c-b54d40e8b2ed.png" alt="image"></p>
<p>We noticed some high coverage areas (peaks), meaning they have many alignments, and some diversity rich areas (lows). There are also some low coverage nodes that appear to form a sequence, which could be areas of high diversity.</p>
<p>The bandage image of the pan-genome was mainly linear, but it had some tangled areas.</p>

