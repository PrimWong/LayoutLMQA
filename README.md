# LayoutLMQA

Empowering youth in financial matters is crucial for their long-term financial well-being and success. Our methodology involves utilising an AI financial planning chatbot for borrowing money and tracking expenses to help empower young individuals in their financial lives. Therefore, the Layout LM Question Answering Model will help youth plan their finances, track how much they spend with a click of a photo, and ask the model any questions!

The LayoutLMQA repository consists of notebooks to train document AI and visual question answering.


![image](https://github.com/PrimWong/LayoutLMQA/assets/145421337/86a7c401-c8d2-4f91-ad89-bde9a081c331)

# Datasets
1. [FUNSD (Form Understanding in Noisy Scanned Documents)](https://guillaumejaume.github.io/FUNSD/)
2. [SQUADv2 (Stanford Question Answering Dataset v2)](https://web.stanford.edu/class/archive/cs/cs224n/cs224n.1194/reports/default/15816213.pdf)
3. [DocVQA (Document Visual Question Answering)](https://arxiv.org/abs/2007.00398)
   
DocVQA is a dataset designed for the task of visual question answering specifically on documents. It involves asking questions about document images, and the models need to answer these questions based on the content within the documents.

![image](https://github.com/PrimWong/LayoutLMQA/assets/145421337/0ccce185-235e-451b-b925-b7da90801b5c)

Additional data collection are pre-processed.

Pre-processing: Data is preprocessed to clean and format it for training. This step includes text and image extraction, layout analysis, and data augmentation to create a suitable training input.

# AI Model | [LayoutLMv3](https://arxiv.org/abs/2204.08387) 
Pre-training for Document AI with Unified Text and Image Masking
![image](https://github.com/PrimWong/LayoutLMQA/assets/145421337/ed97f959-10c2-49ba-8701-3f7a35ce1160)

Word-Patch Alignment Objective: LayoutLMv3 incorporates a word-patch alignment objective. During this stage, the model learns to predict whether an image patch corresponds to a masked word in the text. This helps the model understand the alignment between text and image elements.

Fine-tuning: After pre-training, the model is fine-tuned on specific Document AI tasks on FUNSD and DocVQA dataset. Fine-tuning adapts the model to perform well on tasks like form understanding, receipt analysis, and document classification.

Evaluation: The model's performance is rigorously evaluated using various metrics, F1 score and benchmarks to ensure it meets the desired standards and objectives.

# [Demo Video](https://youtu.be/OZKjBjbqQAg?feature=shared)
![image](https://github.com/PrimWong/LayoutLMQA/assets/145421337/f5131435-e9c6-4ec8-8c34-6ae19b9e6c30)

# References
Document Question Answering. (n.d.). Document Question Answering. https://huggingface.co/docs/transformers/v4.29.0/tasks/document_question_answering
FUNSD. (n.d.). FUNSD. https://guillaumejaume.github.io/FUNSD/
Huang, Y., Lv, T., Cui, L., Lu, Y., & Wei, F. (2022, April 18). LayoutLMv3: Pre-training for Document AI with Unified Text and Image Masking. arXiv.org. https://arxiv.org/abs/2204.08387v3
Mathew, M., Karatzas, D., & Jawahar, C. V. (2020, July 1). DocVQA: A Dataset for VQA on Document Images. arXiv.org. https://arxiv.org/abs/2007.00398v3
Mathew, M., Karatzas, D., & Jawahar, C. V. (2020, July 1). DocVQA: A Dataset for VQA on Document Images. arXiv.org. https://arxiv.org/abs/2007.00398v3
P. (n.d.). LayoutLMQA/layout_LLM_document_question_answering.ipynb at main · PrimWong/LayoutLMQA. GitHub. https://github.com/PrimWong/LayoutLMQA/blob/main/layout_LLM_document_question_answering.ipynb
The Stanford Question Answering Dataset. (2021, June 4). The Stanford Question Answering Dataset. https://rajpurkar.github.io/SQuAD-explorer/
Xu, Y., Li, M., Cui, L., Huang, S., Wei, F., & Zhou, M. (2019, December 31). LayoutLM: Pre-training of Text and Layout for Document Image Understanding. arXiv.org. https://doi.org/10.1145/3394486.3403172
Xu, Y., Xu, Y., Lv, T., Cui, L., Wei, F., Wang, G., Lu, Y., Florencio, D., Zhang, C., Che, W., Zhang, M., & Zhou, L. (2020, December 29). LayoutLMv2: Multi-modal Pre-training for Visually-Rich Document Understanding. arXiv.org. https://arxiv.org/abs/2012.14740v4






