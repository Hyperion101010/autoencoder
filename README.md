# Pre-Evaluation tasks for ATLAS autoencoders.
Use an autoencoder to compress jet event data from 4 to 3 variables from CERN's high energy physics dataset (from ATLAS detector).

The task was divided into two activities:
1. Processing the jet data to convert it into a autoencoder friendly form.
2. To write autoencoder and plot metrics to evaluate performance of the autoencoder.

## Workflow
- The data is first cleaned to only contain 'j' jet entries (check datapreprocessing notebook ).
- It is then pickled and stored in pickle format named as processed_datalabel.pkl
- The autoencoder imports the data and applies necessary normalisation (check dataencoderfastai notebook).
- The model trains on the data.
- Respective metrics are plotted to observe and discuss autoencoder performance.

## Technical Requirements
- FastAI Library https://docs.fast.ai/install.html
- scipy
- corner
- matplotlib
- pandas
- ML environment Dockerfiles for images that contain CERN ATLAS and ML components (https://gitlab.cern.ch/aml/containers/docker)

## References
- Deep Autoencoders for Compression in High Energy Physics by Eric Wulff. [(link)](https://lup.lub.lu.se/student-papers/search/publication/9004751)
- Anomaly detection at the ATLAS detector using a Variational Autoencoder by Remco Volmer.
[(link)](https://www.ru.nl/publish/pages/913395/remco_volmer_01-07-2020.pdf)
- ML compression of ATLAS triggered jet events using autoencoders [(link)](https://github.com/Skelpdar/HEPAutoencoders)

