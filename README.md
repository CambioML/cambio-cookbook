# 👩‍🍳 Cambio Cookbook
Jump into building AI applications with [`Cambio`](https://www.cambioml.com/). This repository contains examples to help you kickstart your AI journey with `Cambio`.

These are built using `Cambio`'s open-source libraries, including [`pykoi`](https://github.com/CambioML/pykoi) and [`uniflow`](https://github.com/CambioML/uniflow).

This repository is a work in progress. We will be adding more examples and tutorials in the coming weeks.

## Examples
These examples dive right into the code with little introduction, so you can get your hands dirty quickly. We recommend you read the [documentation]() or the [tutorials](#tutorials) section to get a better understanding of the concepts and libraries used in these examples.

| Example | Cambio Packages | Description |
| --- | --- | --- |
| [10K Evaluator](./examples/10K%20Evaluator/) | `pykoi`, `uniflow` | A simple example to show how to use Cambio to build a 10K evaluator. |

## Tutorials
These tutorials are designed to help you get started with Cambio. They are written in a step-by-step fashion, and are accompanied by code snippets and explanations.

| Tutorial | Cambio Packages | Description |
| --- | --- | --- |
| Coming Soon! | `pykoi`, `uniflow` | Coming Soon! |

## Installation
To start cooking with `Cambio`, you can install `pykoi` and `uniflow` using `pip` in a `conda` environment.

First, create a conda environment on your terminal using:
```
conda create -n cambio-cookbook python=3.10 -y
conda activate cambio-cookbook  # some OS requires `source activate uniflow`
```


Then, install `pykoi` and `uniflow`:
```
pip3 install pykoi uniflow
```

Finally, install the compatible pytorch based on your OS.
- If you are on a GPU, install [pytorch based on your cuda version](https://pytorch.org/get-started/locally/). You can find your CUDA version via `nvcc -V`.
    ```
    pip3 install --pre torch --index-url https://download.pytorch.org/whl/nightly/cu121  # cu121 means cuda 12.1
    ```
- If you are on a CPU instance,
    ```
    pip3 install torch
    ```

Now, when you go to run the example notebooks, make sure to use the `cambio-cookbook` conda environment when selecting your kernel.

Congrats you have finished the installation!

### API keys
If you are running anything using OpenAI flows, you will have to set up your OpenAI API key.

To do so, create a `.env` file in your root `cambio-cookbook` folder. Then add the following line to the `.env` file:
```
OPENAI_API_KEY=YOUR_API_KEY
```


