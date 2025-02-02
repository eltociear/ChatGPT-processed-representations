# ChatGPT-processed-representations

This repository aims to provide supplementary materials and processed data for the independent research paper (currently under review) titled 'Empowering Few-Shot Recommender Systems with Large Language Models-Enhanced Representations'. The article can be accessed at [arXiv:2312.13557](https://arxiv.org/abs/2312.13557) as a preprint version.

The focus of this article lies in the utilization of Large Language Models (LLMs) for processing explicit textual feedback (i.e., user reviews) to generate representations of users and items. These representations serve as replacements for the model's internally generated embeddings, thereby enhancing the performance of various recommender systems in few-shot scenarios. One crucial step involves generating reinforced representations by leveraging ChatGPT's associations and inferences. We provide corresponding data samples for reference and replication of our findings.

### data description
- **user_train.csv**:  This file contains interaction samples of 100 experimental users, with all samples sorted chronologically and labeled as Train or Test. The test set is recommended to be constructed based on the item ID of the most recent interaction sample (labeled as Test).
- **user_ChatGPT.csv**:  This file contains 100 textual user representations generated by ChatGPT, with the corresponding origin reviews stored in the **user_train.csv** file. The detailed methodology for generating these user representations through prompting is elaborated in the paper.
- **item_train.csv**: This file contains interaction samples for all item IDs present in **user_train.csv**, representing the items that the selected 100 users have engaged with, where each item is associated with up to 10 comments.
- **item_ChatGPT.csv**: This file contains textual item representations generated by ChatGPT, with the corresponding item IDs as presented in the file **user_train.csv**.

The aforementioned dataset is a subset of our experimental dataset. Raw data (including review contents and user IDs) can be access from the Chinese [Douban Movie Review dataset](http://moviedata.csuldw.com/). We sincerely invite you to employ these data for experimental replication and apply them to recommender models beyond the scope of our research paper selectionn 
