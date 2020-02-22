### Current approach

Using DEC (deep embedding clustering) from paper: https://arxiv.org/abs/1511.06335

##### Reasons of trying DEC instead of VaDE
- VaDE latent space cannot converge to mixture-of-gaussians as we expected: visualization of latent space is only a oval cluster ~ 1 gaussian distribution instead of a mixture, so we cannot expect to use common clustering techniques like KMeans or GMM to cluster this latent space.

- Experiment shows that when pre-training VaDE without variational component (training an auto-encoder), the latent space can be used to cluster data.

--> we can use DEC, which is an auto-encoder (not variational autoencoder like VaDE) + clutering loss to cluster our data.

## Some results on clustering

### Hyperparams

Currently, all hyperparameters are set the same for all tested dataset:

- KMERS = [4]
- LMER = 20
- NUM_SHARED_READS = 5: number of overlapping reads to consider an edge in graph (except R1 is 45 and 5).
- ONLY_SEED = True: only uses seed to represent genome signature.
- MAXIMUM_SEED_SIZE = 5000: maximum number of reads in seed set.

### Summary about performance

|Dataset|Precision|Recall|F1-score|
|-------|---------|------|--------|
|S1|0.976|0.976|0.976|
|S2|0.838|0.838|0.838|
|L1|0.961|0.961|0.961|
|L2|0.969|0.969|0.969|
|R1|0.887|0.537|0.669|


### On dataset S1
<figure align="center">
<img src="images/group-s1.png" width="480">
<figcaption>Group representation of dataset.</figcaption>
</figure>

<figure align="center">
<img src="images/seed-s1.png" width="480">
<figcaption>Seed representation of dataset.</figcaption>
</figure>

<figure align="center">
<img src="images/gt-seed-latent-s1.png" width="480">
<figcaption>Latent space representation of dataset (ground truth).</figcaption>
</figure>

<figure align="center">
<img src="images/pred-seed-s1.png" width="480">
<figcaption>Latent space representation of dataset (predicted result).</figcaption>
</figure>


<!-- ============================================================== -->
### On dataset S2
<figure align="center">
<img src="images/group-s2.png" width="480">
<figcaption>Group representation of dataset.</figcaption>
</figure>

<figure align="center">
<img src="images/seed-s2.png" width="480">
<figcaption>Seed representation of dataset.</figcaption>
</figure>

<figure align="center">
<img src="images/gt-seed-latent-s2.png" width="480">
<figcaption>Latent space representation of dataset (ground truth).</figcaption>
</figure>

<figure align="center">
<img src="images/pred-seed-s2.png" width="480">
<figcaption>Latent space representation of dataset (predicted result).</figcaption>
</figure>

<!-- ============================================================== -->
### On dataset L1
<figure align="center">
<img src="images/group-l1.png" width="480">
<figcaption>Group representation of dataset.</figcaption>
</figure>

<figure align="center">
<img src="images/seed-l1.png" width="480">
<figcaption>Seed representation of dataset.</figcaption>
</figure>

<figure align="center">
<img src="images/gt-seed-latent-l1.png" width="480">
<figcaption>Latent space representation of dataset (ground truth).</figcaption>
</figure>

<figure align="center">
<img src="images/pred-seed-l1.png" width="480">
<figcaption>Latent space representation of dataset (predicted result).</figcaption>
</figure>

<!-- ============================================================== -->
### On dataset L2
<figure align="center">
<img src="images/group-l2.png" width="480">
<figcaption>Group representation of dataset.</figcaption>
</figure>

<figure align="center">
<img src="images/seed-l2.png" width="480">
<figcaption>Seed representation of dataset.</figcaption>
</figure>

<figure align="center">
<img src="images/gt-seed-latent-l2.png" width="480">
<figcaption>Latent space representation of dataset (ground truth).</figcaption>
</figure>

<figure align="center">
<img src="images/pred-seed-l2.png" width="480">
<figcaption>Latent space representation of dataset (predicted result).</figcaption>
</figure>

<!-- ============================================================== -->
### On dataset R1
<figure align="center">
<img src="images/group-r1.png" width="480">
<figcaption>Group representation of dataset.</figcaption>
</figure>

<figure align="center">
<img src="images/seed-r1.png" width="480">
<figcaption>Seed representation of dataset.</figcaption>
</figure>

<figure align="center">
<img src="images/gt-seed-latent-r1.png" width="480">
<figcaption>Latent space representation of dataset (ground truth).</figcaption>
</figure>

<figure align="center">
<img src="images/pred-seed-r1.png" width="480">
<figcaption>Latent space representation of dataset (predicted result).</figcaption>
</figure>