# GeoSID: Quantizer-Aware Geometric Shaping for Semantic IDs in Generative Recommendation

Official repository for **GeoSID**, a tokenizer-side geometric shaping framework for Semantic ID-based generative recommendation.

> 🚧 **Code coming soon.**  
> We are preparing the implementation, configuration files, and reproduction instructions for release.

## Overview

GeoSID improves Semantic ID construction by reshaping item representations before code assignment while keeping the downstream generative recommender unchanged. Its key idea is to align geometric regularization with the decomposition structure of the tokenizer:

- **Residual quantization:** distribution shaping is applied to residual-level representations.
- **Product quantization:** distribution shaping is applied to OPQ-aligned PQ blocks.
- **Plug-and-play design:** the item encoder and downstream recommendation pipeline remain unchanged.

Experiments on multiple public recommendation datasets and Semantic ID backbones show improvements of up to **8.13% in Recall@10** and **6.91% in NDCG@10**. Further analysis indicates more balanced code usage and fewer prefix-level Semantic ID collisions.
