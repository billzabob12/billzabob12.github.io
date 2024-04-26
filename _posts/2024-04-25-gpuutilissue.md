# GPU Memory Usage Maxing Out

I have run into an issue when trying to train a resnet-18 neural net. When using various batch sizes and plotting the GPU utilisation and memory usage, I get the following  output:

![GPU Loading](/images/gpu_loading.png)

There are 5 different batch sizes being run (16, 32, 64, 128, 256) and the memory usage and GPU utilsation is the final batch run. It is clear to see that the GPU utilisation is much lower for the 256 batch size when compared to the 128 batch size and the same can be said for the memory usage. I think this may be due to my GPU not having enough memory so it is unable to actually train the model with a batch size of 256 and instead uses smaller batches. This doesn't explain the low utilisation though. I will continue to investigate this and if I find a solution or why this is occuring I will update this post.