# Cloud computing

In the [first notebook](https://github.com/JulienfLeBoucher/OC_cloud_computing/blob/main/local.ipynb), I discovered and experimented with Apache Spark locally.

Then, I created a [second notebook](https://github.com/JulienfLeBoucher/OC_cloud_computing/blob/main/cloud_image_processing.ipynb) slightly adapted to be executed in an AWS EMR cluster
with a pyspark kernel.

In the end of the first notebook and in the [third notebook](https://github.com/JulienfLeBoucher/OC_cloud_computing/blob/main/not_distributed_plus_comparison.ipynb), I assessed performance differences
between running the image processing chain via Spark and via a classic tensorflow pipeline and tried
to understand where the value variations came from (pre-processing steps with different resize functions). I also quickly evaluated the quality of the online spark processing with t-SNE visualizations.

On the small dataset used (320 images), Spark was 10 times slower (see the [presentation](https://github.com/JulienfLeBoucher/OC_cloud_computing/blob/main/presentation_p8.pdf) to see the EMR cluster configuration). 

The remaining files of that repository are configuration files placed on my S3 bucket which I referred to when configuring the EMR cluster.