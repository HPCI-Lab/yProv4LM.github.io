# yProv4ML

[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)

This library is part of the yProv suite, and provides a unified interface for logging and tracking provenance information in machine learning experiments, both on distributed as well as large scale experiments. 

It allows users to create provenance graphs from the logged information, and save all metrics and parameters to json format.

## Data Model

![Data Model](./assets/prov4ml.datamodel.png)

## Example

![Example](./assets/example.svg)

The image shown above has been generated from the [example](./examples/mlflow_lightning.py) program provided in the ```example``` directory.

## Metrics Visualization

![Loss and GPU Usage](./assets/System_Metrics.png)

![Emission Rate](assets/Emission_Rate.png) 

## Experiments and Runs

An experiment is a collection of runs. Each run is a single execution of a machine learning model. 
By changing the ```experiment_name``` parameter in the ```start_run``` function, the user can create a new experiment. 
All artifacts and metrics logged during the execution of the experiment will be saved in the directory specified by the experiment ID. 

Several runs can be executed in the same experiment. All runs will be saved in the same directory (according to the specific experiment name and ID).

# Documentation

For detailed information, please refer to the [Documentation](https://hpci-lab.github.io/yProv4ML.github.io/)

<!-- - [Installation](./wiki/installation.md)
- [Setup](./wiki/setup.md)
- [Provenance Graph](./wiki/prov_graph.md)
- [Logging](./wiki/logging.md)
- [Prov Collection](./wiki/prov_collection.md)
- [Carbon Metrics](./wiki/carbon.md)
- [System Metrics](./wiki/system.md)
- [Time Metrics](./wiki/time.md)
- [Registering Metrics](./wiki/registering_metrics.md)
- [Usage with PyTorch](./wiki/usage_pytorch.md)
- [Usage with Lightning](./wiki/usage_lightning.md)
- [Usage with ItwinAI Logger](./wiki/usage_itwinAI_logger.md) -->

# Contributors

- [Gabriele Padovani](https://github.com/lelepado01)
- [Luca Davi](https://github.com/lucadavii)
- [Sandro Luigi Fiore](https://github.com/sandrofioretn)