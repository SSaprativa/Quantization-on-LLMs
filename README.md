
# Quantization on LLMs

This repository demonstrates how to apply linear quantization to large language models using PyTorch. Quantization is a process that reduces the model size and inference latency by converting high-precision weights to lower precision. This project explores quantization with random scale and zero points.

### Features
**Linear Quantization**: Implemented linear quantization using a custom scale and zero point.\
**Example Demonstrations**: The notebook contains practical examples of quantizing tensors using the described method.\
**Custom Tensor Operations**: The code performs operations such as scaling, rounding, and clamping to achieve quantization.

## Requirements
Python: 3.x\
PyTorch: 1.x or later

## Model Improvements
This project not only explores quantization techniques but also includes optimizations applied to existing in-built models. The goal of these optimizations is to enhance the performance and efficiency of the models in terms of both space and computational requirements.

#### *Salesforce/codegen-350M-mono* Model Optimization
**Space Optimization**: 
The Salesforce/codegen-350M-mono model was optimized for reduced memory consumption, which is crucial for deployment in resource-constrained environments. Techniques like weight quantization and pruning were applied to achieve a more compact model without significant loss of accuracy.

**Results**: The space optimization resulted in a 49% reduction in the model size, making it more suitable for deployment in environments with limited resources.

**Inference Speed**: By implementing these optimizations, the inference time was improved, making the model more suitable for real-time applications.
#### *facebook/detr-resnet-50* Model Optimization
**Memory Efficiency**: The facebook/detr-resnet-50 model was optimized to decrease its memory footprint while maintaining its high performance in object detection tasks.

**Results**: The space optimization resulted in a 31% reduction in the model size, making it more suitable for deployment in environments with limited resources.

**Custom Quantization**: A custom quantization approach was applied to further reduce the model size, enabling faster inference while preserving the integrity of the detection outputs.

### Conclusion
This project successfully demonstrates the application of advanced quantization techniques to large language models, achieving significant space and memory optimizations. By focusing on models like Salesforce/codegen-350M-mono and facebook/detr-resnet-50, we have shown how targeted optimizations can lead to substantial reductions in model size without compromising performance. These improvements not only make the models more efficient but also extend their applicability to a wider range of environments, including those with limited computational resources.

The quantization methods and optimizations presented here are crucial steps toward making large language models more accessible and practical for real-world applications. As the field of AI continues to evolve, such techniques will be increasingly important for deploying sophisticated models in diverse and resource-constrained scenarios.

We hope this work serves as a valuable resource for developers and researchers looking to enhance the efficiency of their models. Contributions and further improvements are welcome, as the journey to optimizing AI models is ongoing and collaborative.







