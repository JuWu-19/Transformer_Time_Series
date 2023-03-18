####  Transformer for Time Series
This project aims to use transformer encoder module to model the nonlinear relationships between the input and output data of long-term memory.

For time-series input-output regression task, the transformer has the following explicit advantages compared to RNNs.
-   Parallel processing: Transformers can process input sequences in parallel, which makes them much faster than RNNs for long sequences.
-   Longer context: Transformers can capture longer-term dependencies in the input sequence than RNNs, which makes them better suited for tasks that require modeling long-range dependencies.
- Attention mechanism: The attention mechanism used in Transformers allows them to selectively focus on relevant parts of the input sequence, which helps them handle variable-length sequences and capture more complex relationships between elements of the sequence.
- Position encoding: Transformers use position encoding to provide each input element with a unique positional embedding, which enables the model to take into account the position of each element in the sequence. This is important for tasks that require modeling sequential data, and helps the model distinguish between different positions in the sequence explicitly.

The model is as folllows
$$\hat{y}(T) = Trans(u(T),\ldots,u(T-N)).$$
where $N$ is the length of the past information of input $u$ that has impact on the output $\hat{y}$.

The project consists of three parts

1). A toy transformer encoder to model relationships between input and output
2). The input-output dataset of a toy example
3). The training procedure and fitting results of the first 50 epoches.
