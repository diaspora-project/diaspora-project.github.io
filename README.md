## Resilience-enabling services for science from HPC to edge

An [**AI-guided simulation campaign**](Text/applications.md) that engages computers at multiple sites to evaluate many small molecules for use against a new pathogen. A [**real-time data analysis pipeline**](Text/applications.md) that processes data from a scientific instrument so as to enable experimental steering. A [**multi-messenger astronomy application**](Text/applications.md) that integrates data from observational and simulation sites to detect and respond rapidly to rare astronomical events. Each of these mission-critical applications depends on distributed computation for its success and is thus easily subject to disruptions due to  failures, disruptions, and other anomalies. 

Our goal in the Diaspora project is to develop new methods for building next-generation resilient scientific applications capable of executing in an increasingly integrated research infrastructure. Experience in other domains, such as public clouds, has demonstrated the power of event-driven communication as a foundation for resilient solutions. However, such approaches are under-exploited in scientific computing due to different scales, scope, and service level requirements. We hypothesize that:

> Addressing the resilience needs of a broad set of DOE applications requires methods for gaining knowledge of resources and applications and for translating that knowledge into action. 
These two needs can be met by establishing a **unifying event fabric** that extends across sites, facilities, and computations to provide timely, reliable, and accurate information about data, application, and resource status, and by developing **resilience services** that leverage information provided by this fabric to meet broad classes of resilience needs.

Thus, as outlined in the figure, we are working to create a **hierarchical event fabric** (encompassing, via **Mofka**, HPC); to develop **resilience services** that build on event fabric capabilities to provide, e.g., resilient compute pools and streaming; and to evaluate these new capabilities in **scientific applications** such as those listed above. 

<p align="center" width="100%">
    <img width="60%" src="Diaspora.png">
</p>

Project participants include:
* At [Texas Tech](https://www.ttu.edu), [Alessandra Corsi](https://www.depts.ttu.edu/phas/People/Faculty/bio_corsi/bio_corsi.php)
* At [SLAC](https://slac.stanford.edu), Ryan Coffee and Jana Thayer
* At [ORNL](https://www.ornl.gov), Nagi Rao and Anees Najjar
* At [Argonne](https://www.anl.gov): Ian Foster, Tekin Bicer, Phil Carns, Kyle Chard, Ryan Chard, Matthieu Dorier, Eliu Huerta, Raj Kettimuthu, Bogdan Nicolae, Rob Ross, Justin Wozniak.

We are looking for people who want to help us build out these solutions: postdocs, students, visiting scientists, collaborators, and others. If you think that you might be interested, please get in touch with [Ian Foster](mailto:foster@anl.gov). We look forward to hearing from you! 

And just for fun, a [description of the project suitable for a kindergartener](Text/kindergartener.md).

---

Diaspora involves researchers at Argonne National Laboratory, Oak Ridge National Laboratory, SLAC, and Texas Tech University, and is supported by a grant from the US Department of Energy's [Office of Advanced Scientific Computing Research](https://science.osti.gov/ascr), under program manager [Margaret Lentz](https://science.osti.gov/ascr/About/Staff). Access at [diaspora-project.github.io](https://diaspora-project.github.io). For more information contact [Ian Foster](mailto:foster@anl.gov). 


