# How RAPTOR Works: 

## Overview: 
RAPTOR (Recursive Augmented Processing Tree for Retrieval) is a novel technique for enhancing text retrieval and comprehension, especially for long texts with complex structures and themes. It aims to provide a balance between broad thematic understanding and granular details. 

## Stage 1: Text Segmentation 
The first stage involves dividing the retrieval corpus into short, contiguous texts of approximately 100 words each. This segmentation process is similar to traditional retrieval augmentation techniques and helps in creating manageable chunks for further processing. 

## Stage 2: Tree Structure Construction 
RAPTOR then builds a recursive tree structure from the segmented texts. This tree is designed to capture the hierarchical nature of the text, with nodes representing thematic concepts and their relationships. Nodes are grouped based on semantic similarity, allowing for a more meaningful organization than simply following the order of the text. 

## Stage 3: Node Selection and Retrieval 
When a question is asked, RAPTOR traverses its tree structure to select relevant nodes that provide context and answers. These nodes can belong to different layers of the tree, depending on the level of detail required by the question. This adaptive retrieval process demonstrates RAPTOR's ability to understand the text comprehensively. 

For example, in Figure 4, for the question, "What is the central theme of the story?" RAPTOR retrieves an upper-level node containing the sentence, "This story is about the power of human connection...," capturing the main theme. 

## Stage 4: Contextual Understanding and Exhaustiveness 
RAPTOR's strength lies in its ability to provide exhaustive and relevant information. By leveraging the tree structure, it can often retrieve context that encompasses the answers provided by other retrievers, like DPR, either directly or within higher-layer summaries. This ensures that the information presented is comprehensive and supports better performance on downstream tasks. 

## Stage 5: Adaptability and Compatibility 
Finally, RAPTOR is designed to be adaptable and compatible. It can be combined with any retriever, and its recursive tree structure allows for flexible information retrieval, ensuring that it consistently outperforms other retrievers across various datasets and metrics, as demonstrated in the experiments. 

In summary, RAPTOR enhances text retrieval by constructing a recursive tree structure that captures the semantic depth and connections within the text. Its node selection process, based on question granularity, enables it to provide exhaustive and relevant context, making it a powerful tool for improving comprehension and performance on downstream tasks.
