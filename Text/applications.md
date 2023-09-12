# Motivating applications

## Long-term campaigns

These applications perform many computations and/or experiments ("tasks") over extended periods, using multiple computers and laboratories.
The status of current tasks and the results of past tasks must be repeatedly updated and consulted (e.g., to compute diagnostics, train AI surrogates, choose the next task) as the campaign proceeds.
While instances of this pattern (e.g., high energy physics data analysis, self-driving laboratories, molecular dynamics) differ in computational structure, data rates, resilience requirements, etc., 
the following example is representative: 

* **Goal**: AI-guided molecular dynamics studies to identify small-molecule SARS-CoV-2 therapeutics.
* **Environment**: DOE HPC systems.
* **Service levels**: 1000 tasks per hour, AI training every 600~s, preserve task outputs. 
* **Anomalies**: Failure or reduced availability of individual systems; network partitions; loss of state.
* **Responses**: Load migration, state replication.

In one recent representative example, an Argonne-led team developed a 2022 Gordon Bell-winning AI-guided simulation campaign application 
that involved thousands of simulations and AI training and inference tasks totaling 1.6x10<sup>21</sup> FP16 and FP32 floating point operations on 
large GPU clusters at ALCF and NVIDIA and on interconnected Cerebras CS-2 systems: see [Zvyagin et al., 2022](https://www.biorxiv.org/content/10.1101/2022.10.10.511571v1).

The following figure, from [Ward et al., 2003](https://arxiv.org/abs/2303.08803), illustrates an AI-guided simulation campaign that combines AI training and inference on GPUs that steer simulations on CPUs. 

<p align="center" width="100%">
    <img width="50%" src="Images/ColmenaHetero.png">
</p>

## Time-sensitive applications

These applications have end-to-end urgency, for example due to a need to provide real-time feedback to an experiment
or to train AI models that are deployed at an instrument for steering.
Such pipelines must satisfy temporal demands despite resource failures and changing computational demands, among other factors.
E.g.:

* **Goal**: Rapid detection and response to events in instrument data stream.
* **Environment**: Synchrotron light sources, HPC systems.
* **Service levels**: Analyze multi-GB/s data stream with <10 s latency, preserve raw and processed data. 
* **Anomalies**: Failure or reduced availability of HPC systems, networks; increased need.
* **Responses**: Switch computers; substitute analysis.

The following figure (see e.g. [Liu et al., 2022](https://arxiv.org/pdf/2105.13967.pdf)) shows data center HPC being used used to train ML models for fast data filtering at a synchrotron instrument.

<p align="center" width="100%">
    <img width="70%" src="Images/dcai_flow.png">
</p>

## Distributed data integration applications 

These applications combine and analyze data from multiple sources. For example, in multi-messenger astronomy (MMA), 
the need to detect and respond to unusual transient events in multiple cosmic messengers (gravitational wave, electromagnetic, high-energy particles 
from different instruments leads to a federated learning problem. 

* **Goal**: Federated training and inference on data from multiple sources.
* **Environment**: Astronomical observatories, HPC systems,
* **Service levels**: Training times, ability to retrieve raw and processed data. 
* **Anomalies**: Failure or reduced availability of individual systems, and LAN/WAN connections.
* **Responses**: Migrate computation, redundant network, substitute surrogates, drop sources.

The following figure illustrates how to accelerate discovery from multi-messenger sources, 
we apply federated learning over messengers to produce a foundation model.

<p align="center" width="100%">
    <img width="70%" src="Images/fed_len_MMA_ian.png">
</p>

