### Summary about performance - 20/03/2020


### Parameters
- Network architecture (applied for all dataset): 136-500-1000-10.
- Learning rate: using default learning rate (0.01).
- Number of shared read for buidling graph: 5 for L, S dataset; 45 for R dataset.
- Maximum seed size: 200.
- LMER: 20.
- KMERS: 4.

|Dataset|Precision|Recall|F1-score|F1 BiMeta|F1 MetaProb|
|-------|---------|------|--------|---------|-----------|
|S1|0.991|0.991|0.991|0.978|0.991|
|S2|0.924|0.924|0.924|0.581|0.901|
|S3|0.969|0.969|0.969|0.978|0.928|
|S4|0.988|0.988|0.988|0.994|0.908|
|S5|0.884|0.884|0.884|0.690|0.823|
|S6|0.994|0.994|0.994|0.858|0.970|
|S7|0.702|0.767|0.733|0.843|0.782|
|S8|0.833|0.581|0.685|0.743|0.769|
|S9|0.727|0.657|0.690|0.791|0.719|
|S10|0.584|0.498|0.538|0.429|0.495|


|Dataset|Precision|Recall|F1-score|F1 BiMeta|F1 MetaProb|
|-------|---------|------|--------|---------|-----------|
|L1|0.982|0.982|0.982|0.980|0.984|
|L2|0.990|0.990|0.990|0.980|0.992|
|L3|0.988|0.988|0.988|0.986|0.993|
|L4|0.991|0.991|0.991|0.987|0.986|
|L5|0.988|0.988|0.988|0.991|0.983|
|L6|0.985|0.985|0.985|0.990|0.984|


|Dataset|Precision|Recall|F1-score|F1 BiMeta|F1 MetaProb|
|-------|---------|------|--------|---------|-----------|
|R1|0.943|0.943|0.943|0.609|0.971|
|R2|0.858|0.858|0.858|0.773|0.968|
|R3|0.814|0.814|0.814|0.780|0.928|
|R4|0.992|0.992|0.992|0.992|0.993|


#### Visualization of Lx dataset

| | | |
|:-------------------------:|:-------------------------:|:-------------------------:|
|<img width="1604" alt="seed-L1" src="20200320images/seed-L1.png"> L1 seeds' representation |<img width="1604" alt="gt-seed-latent" src="20200320images/gt-seed-latent-L1.png"> L1 latent groundtruth |<img width="1604" alt="pred-seed-latent" src="20200320images/pred-seed-latent-L1.png"> L1 latent prediction|
|<img width="1604" alt="seed-L3" src="20200320images/seed-L3.png"> L3 seeds' representation |<img width="1604" alt="gt-seed-latent" src="20200320images/gt-seed-latent-L3.png"> L3 latent groundtruth |<img width="1604" alt="pred-seed-latent" src="20200320images/pred-seed-latent-L3.png"> L3 latent prediction|
|<img width="1604" alt="seed-L5" src="20200320images/seed-L5.png"> L5 seeds' representation |<img width="1604" alt="gt-seed-latent" src="20200320images/gt-seed-latent-L5.png"> L5 latent groundtruth |<img width="1604" alt="pred-seed-latent" src="20200320images/pred-seed-latent-L5.png"> L5 latent prediction|
|<img width="1604" alt="seed-L6" src="20200320images/seed-L6.png"> L6 seeds' representation |<img width="1604" alt="gt-seed-latent" src="20200320images/gt-seed-latent-L6.png"> L6 latent groundtruth |<img width="1604" alt="pred-seed-latent" src="20200320images/pred-seed-latent-L6.png"> L6 latent prediction|


#### Visualization of Rx dataset

| | | |
|:-------------------------:|:-------------------------:|:-------------------------:|
|<img width="1604" alt="seed-R1" src="20200320images/seed-R1.png"> R1 seeds' representation |<img width="1604" alt="gt-seed-latent" src="20200320images/gt-seed-latent-R1.png"> R1 latent groundtruth |<img width="1604" alt="pred-seed-latent" src="20200320images/pred-seed-latent-R1.png"> R1 latent prediction|
|<img width="1604" alt="seed-R2" src="20200320images/seed-R2.png"> R2 seeds' representation |<img width="1604" alt="gt-seed-latent" src="20200320images/gt-seed-latent-R2.png"> R2 latent groundtruth |<img width="1604" alt="pred-seed-latent" src="20200320images/pred-seed-latent-R2.png"> R2 latent prediction|
|<img width="1604" alt="seed-R3" src="20200320images/seed-R3.png"> R3 seeds' representation |<img width="1604" alt="gt-seed-latent" src="20200320images/gt-seed-latent-R3.png"> R3 latent groundtruth |<img width="1604" alt="pred-seed-latent" src="20200320images/pred-seed-latent-R3.png"> R3 latent prediction|
|<img width="1604" alt="seed-R4" src="20200320images/seed-R4.png"> R4 seeds' representation |<img width="1604" alt="gt-seed-latent" src="20200320images/gt-seed-latent-R4.png"> R4 latent groundtruth |<img width="1604" alt="pred-seed-latent" src="20200320images/pred-seed-latent-R4.png"> R4 latent prediction|


#### Visualization of Sx dataset

| | | |
|:-------------------------:|:-------------------------:|:-------------------------:|
|<img width="1604" alt="seed-S1" src="20200320images/seed-S1.png"> S1 seeds' representation |<img width="1604" alt="gt-seed-latent" src="20200320images/gt-seed-latent-S1.png"> S1 latent groundtruth |<img width="1604" alt="pred-seed-latent" src="20200320images/pred-seed-latent-S1.png"> S1 latent prediction|
|<img width="1604" alt="seed-S2" src="20200320images/seed-S2.png"> S2 seeds' representation |<img width="1604" alt="gt-seed-latent" src="20200320images/gt-seed-latent-S2.png"> S2 latent groundtruth |<img width="1604" alt="pred-seed-latent" src="20200320images/pred-seed-latent-S2.png"> S2 latent prediction|
|<img width="1604" alt="seed-S3" src="20200320images/seed-S3.png"> S3 seeds' representation |<img width="1604" alt="gt-seed-latent" src="20200320images/gt-seed-latent-S3.png"> S3 latent groundtruth |<img width="1604" alt="pred-seed-latent" src="20200320images/pred-seed-latent-S3.png"> S3 latent prediction|
|<img width="1604" alt="seed-S4" src="20200320images/seed-S4.png"> S4 seeds' representation |<img width="1604" alt="gt-seed-latent" src="20200320images/gt-seed-latent-S4.png"> S4 latent groundtruth |<img width="1604" alt="pred-seed-latent" src="20200320images/pred-seed-latent-S4.png"> S4 latent prediction|
|<img width="1604" alt="seed-S5" src="20200320images/seed-S5.png"> S5 seeds' representation |<img width="1604" alt="gt-seed-latent" src="20200320images/gt-seed-latent-S5.png"> S5 latent groundtruth |<img width="1604" alt="pred-seed-latent" src="20200320images/pred-seed-latent-S5.png"> S5 latent prediction|
|<img width="1604" alt="seed-S6" src="20200320images/seed-S6.png"> S6 seeds' representation |<img width="1604" alt="gt-seed-latent" src="20200320images/gt-seed-latent-S6.png"> S6 latent groundtruth |<img width="1604" alt="pred-seed-latent" src="20200320images/pred-seed-latent-S6.png"> S6 latent prediction|
|<img width="1604" alt="seed-S7" src="20200320images/seed-S7.png"> S7 seeds' representation |<img width="1604" alt="gt-seed-latent" src="20200320images/gt-seed-latent-S7.png"> S7 latent groundtruth |<img width="1604" alt="pred-seed-latent" src="20200320images/pred-seed-latent-S7.png"> S7 latent prediction|
|<img width="1604" alt="seed-S8" src="20200320images/seed-S8.png"> S8 seeds' representation |<img width="1604" alt="gt-seed-latent" src="20200320images/gt-seed-latent-S8.png"> S8 latent groundtruth |<img width="1604" alt="pred-seed-latent" src="20200320images/pred-seed-latent-S8.png"> S8 latent prediction|
|<img width="1604" alt="seed-S9" src="20200320images/seed-S9.png"> S9 seeds' representation |<img width="1604" alt="gt-seed-latent" src="20200320images/gt-seed-latent-S9.png"> S9 latent groundtruth |<img width="1604" alt="pred-seed-latent" src="20200320images/pred-seed-latent-S9.png"> S9 latent prediction|
|<img width="1604" alt="seed-S10" src="20200320images/seed-S10.png"> S10 seeds' representation |<img width="1604" alt="gt-seed-latent" src="20200320images/gt-seed-latent-S10.png"> S10 latent groundtruth |<img width="1604" alt="pred-seed-latent" src="20200320images/pred-seed-latent-S10.png"> S10 latent prediction|
