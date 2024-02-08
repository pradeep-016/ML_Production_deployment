# TFX Pipeline for Vertex Pipelines in Google Cloud

This repository contains a TFX (TensorFlow Extended) pipeline for building and deploying machine learning models using Vertex Pipelines in Google Cloud.

## Overview

TFX is an end-to-end platform for deploying production machine learning pipelines. Vertex Pipelines is a managed service provided by Google Cloud for building, deploying, and monitoring machine learning pipelines.

This project demonstrates how to set up a TFX pipeline using Vertex Pipelines to train, validate, and deploy machine learning models on Google Cloud.

## Features

- Utilizes TFX components such as ExampleGen, Transform, Trainer, and Pusher.
- Integrates with Vertex AI for model training and deployment.
- Implements custom components for data preprocessing and feature engineering.
- Includes a sample dataset and model for demonstration purposes.

## Setup

1. Clone this repository:

```bash
git clone https://github.com/pradeep-016/ML_Production_deployment.git
cd tfx-vertex-pipeline
```

2. Install the necessary dependencies:

```bash
pip install -r requirements.txt
```

3. Configure your Google Cloud project and authenticate with the gcloud command-line tool:

```bash
gcloud init
```

4. Set up your GCP environment variables:

```bash
export PROJECT_ID=your_project_id
export REGION=your_region
```

5. Customize the pipeline configuration in `pipeline/config.py` according to your project requirements.

6. Run the pipeline using the following command:

```bash
python -m pipeline.run_pipeline
```

7. Monitor the pipeline execution in the Vertex AI Console.

## Contributing

Contributions to this project are welcome! If you find any bugs or have suggestions for improvement, please open an issue or submit a pull request.

