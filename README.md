# CineQuest: A Movie-Based Question-Answering Dataset with varying complexity level.
This work presents CineQuest, a dataset comprising approximately 170K question–answer pairs derived from Hollywood and Bollywood movies. The questions span various aspects such as plot, production, cast, and more, and are categorised into three types: Yes/No, single-correct MCQs, and multiple-correct MCQs, each reflecting different levels of complexity.

We propose a scalable and minimally supervised method for generating large QA datasets using knowledge graphs (KGs). By leveraging large language models (LLMs), the approach constructs KGs from textual segments and generates questions based on node–edge–node triplets. This framework is capable of producing a wide range of question types, with complexity governed by the hop lengths within the KG. The automation and scalability of the method significantly reduce the need for manual effort, enabling the standardised creation of QA datasets.

To ensure dataset quality, we conducted human evaluations and benchmarked state-of-the-art language models (LMs) on CineQuest to assess their understanding of movie knowledge. While the dataset is not directly applied to recommendation systems, it serves as evidence of our automated pipeline’s ability to generate high-quality, domain-specific QA data. Overall, this work highlights the effectiveness of KG-based methods for automated dataset creation and evaluating LMs’ movie-domain knowledge.

<img width="526" height="581" alt="download" src="https://github.com/user-attachments/assets/fc15fa00-f9d1-46a7-a3e3-c13e1db38413" />



# Dataset Folder and its file structure
The Questions_Answers folder in the Dataset folder follows the structure presented in the above figure. In the folder, there are two categories, Bollywood and Hollywood. Each category has three different Hop folders for three different complexities: (i) Simple Q/A (Hop\_1), (ii) Moderate Q/A (Hop\_2), and (iii) Complex Q/A (Hop\_3). In each Hop folder, there are again three different types of question folders: (a) Yes/No, (b) MCQ\_Single\_Correct, and (c) MCQ\_Multiple\_Correct. Finally, in each of the question folders, the question files of movies are stored in .json file format. The JSON file names have been formatted as ***MovieName_YoR_aspect.json*** for better question referencing. Each file contains the questions with actual answers generated from the respective movie aspect.

Besides that, the Dataset folder also contains the Node-Edge information of each movie from different categories by following the same nomenclature. 
