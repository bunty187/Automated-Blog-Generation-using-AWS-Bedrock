# How RAPTOR Works: A Step-by-Step Explanation 

## Introduction
RAPTOR is a novel retrieval mechanism that has been designed to address the challenges of semantic depth and connection in reading comprehension tasks. It builds upon the idea that long texts often contain subtopics and hierarchical structures, and aims to provide more relevant and exhaustive information retrieval for better performance on downstream tasks. 

## Step 1: Text Segmentation 
The first step in the RAPTOR process is to segment the retrieval corpus into short, contiguous texts of a length of around 100 words. This is a standard technique used in retrieval augmentation, ensuring that the text is broken down into manageable and consistent segments for processing. 

## Step 2: Recursive Tree Structure 
The unique aspect of RAPTOR is its recursive tree structure. After segmentation, RAPTOR builds a tree by grouping these short texts (or nodes) based on their semantic similarity, not just their order in the text. This allows for the capture of subtopics and hierarchical relationships within the text. 

## Step 3: Node Selection 
When a question is posed to RAPTOR, it traverses the tree structure to select the most relevant nodes to answer the question. These nodes are chosen from different layers of the tree, depending on the level of granularity required by the question. This allows RAPTOR to provide a more nuanced and exhaustive response, capturing both broader thematic ideas and specific details. 

## Step 4: Integration with LLMs 
RAPTOR can be integrated with Large Language Models (LLMs) to enhance their performance. In the experiments, RAPTOR was combined with GPT-3, GPT-4, and UnifiedQA to demonstrate its effectiveness. 

## Step 5: Performance Evaluation 
The performance of RAPTOR is then evaluated using standard metrics such as ROUGE-L, BLEU-1, BLEU-4, METEOR, and F-1 Match scores. These metrics measure the quality of the retrieved information and its relevance to the question asked. 

## Conclusion
By following these steps, RAPTOR provides a more comprehensive and nuanced understanding of the text, outperforming traditional retrieval mechanisms like BM25 and DPR. This results in improved performance on a range of downstream tasks, particularly those requiring information synthesis and understanding of complex textual structures. 

--- 

For further details on RAPTOR's implementation and experimental results, please refer to the accompanying research paper. This step-by-step guide provides a high-level overview of how RAPTOR works and the key processes involved in its innovative retrieval approach.
