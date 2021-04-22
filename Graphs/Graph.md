Graph is a set of annotated nodes and edges.
They tend to be heterogenous - they have more than one type of node and edge.

A lot of problems can be described as graphs - images in the computer vision can be described as a graph of nodes which are pixels and edges are neighbourgh relationships between them.

Important tool in image understanding are convolutional network layers that create new views of data by taking into account the neighbourhood of each pixel. In the NLP the transformers are analogous to that - they use the local context of each word in the string. This concept of locality is essential for deep learning algorithms.

Examples of tools for managing graphs: Amazon Neptune, Azure CosmosDB, W3C RDF + SPARQL, Apache Tinkerpop, Boost Graph Library, NetworkX, Deep Graph Library (DGL)

DGL message passing is an important feature for convolution an transformers on graphs. Messages are associated with edges and they take a value from source note and deliver in to the destination node. Defined reduce function on the destination node processes these messages and updates attributes of the destination node accordingly.

## Knowledge graphs

One approach to building knowledge graphs from documents in to find named entities in each block of the document - which may be for example a paragraph, then create a node for the block and connect it with nodes of all entities that were recognized in the block.







