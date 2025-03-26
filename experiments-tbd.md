
## First Experiment with Neuron
Study our architecture: https://awsdocs-neuron.readthedocs-hosted.com/en/latest/general/arch/index.html
Run a few micro benchmarks: https://github.com/aws-neuron/aws-neuron-samples/blob/master/torch-neuronx/microbenchmark/microbenchmark.ipynb
Run the profiler: https://awsdocs-neuron.readthedocs-hosted.com/en/latest/tools/neuron-sys-tools/neuron-profile-user-guide.html

Generate a graph of matmult performance for different matmult sizes
X axis should be matrix size (choose the dimensions of interest, could be square matrices or not)
Y axis should be ‘achieved TFLOPS’ (achievable performance)
Parallel compilation might be useful (‘neuron_parallel_compile python3 matmul.py’)

Generate a neuron-profile for one of the runs: https://awsdocs-neuron.readthedocs-hosted.com/en/latest/tools/neuron-sys-tools/neuron-profile-user-guide.html

Generate an HTML view, browse through the profile, see if it’s intuitive

Train a medium-sized LLaMA 7B model with 7B parameters: https://github.com/aws-neuron/aws-neuron-parallelcluster-samples/blob/master/examples/jobs/neuronx-nemo-megatron-llamav2-job.md

No need to train to completion, but let’s see a clear loss-convergence trend




