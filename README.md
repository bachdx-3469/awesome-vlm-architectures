# Awesome-VLM-Architectures
<details> 
  <summary><h3>LLaVA</h3></summary> 
    <table>
    <thead>
    <tr>
    <th>Title</th>
    <th>Architecture.Overview</th>
    <th>Architecture.Components</th>
    <th>Training.Methods</th>
    <th>Alignment.Techniques</th>
    <th>Alignment.Fusion Methods</th>
    <th>Datasets.Used</th>
    <th>Datasets.Purpose</th>
    </tr>
    </thead>
    <tbody>
    <tr>
    <td><a href="https://arxiv.org/abs/2304.08485">LLaVA: Large Language and Vision Assistant</a></td>
    <td>LLaVA combines a pre-trained language model (LLM) with a visual model to leverage the capabilities of both for multimodal understanding. It integrates a vision encoder with a language decoder for processing and understanding language-image instruction data.</td>
    <td>Key components include the CLIP visual encoder for image feature extraction and the Vicuna language model for processing language instructions. A simple linear layer connects image features to the word embedding space, aligning visual and language representations.</td>
    <td>LLaVA is trained using a two-stage instruction-tuning procedure. The first stage involves pre-training for feature alignment, utilizing a filtered dataset to align image features with LLM word embeddings. The second stage involves fine-tuning both the projection layer and LLM end-to-end on specific tasks like a multimodal chatbot and Science QA, focusing on enhancing the model&#39;s instruction-following capabilities.</td>
    <td>The model employs instruction-tuning to align text-image data, generating multimodal instruction-following data using GPT-4. This involves converting image-text pairs into formats suitable for instruction-following tasks.</td>
    <td>A trainable projection matrix is used to convert visual features into language embedding tokens, aligning image and language representations within the same dimensional space. This facilitates encoding vision and text together effectively.</td>
    <td>Filtered CC3M, LLaVA-Instruct-158K, ScienceQA</td>
    <td>Filtered CC3M is used for pre-training to align visual and language features. LLaVA-Instruct-158K, a dataset generated using GPT-4, is used for fine-tuning on multimodal tasks. ScienceQA is utilized to evaluate the model&#39;s performance on multimodal reasoning tasks.</td>
    </tr>
    </tbody>
    </table>
</details>
<details>  
  <summary><h3>LLaVA 1.5</h3></summary> 
    <table>
    <thead>
    <tr>
    <th>Title</th>
    <th>Architecture.Overview</th>
    <th>Architecture.Components</th>
    <th>Training.Methods</th>
    <th>Alignment.Techniques</th>
    <th>Alignment.Fusion Methods</th>
    <th>Datasets.Used</th>
    <th>Datasets.Purpose</th>
    </tr>
    </thead>
    <tbody>
    <tr>
    <td><a href="https://arxiv.org/abs/2310.03744">Improved Baselines with Visual Instruction Tuning</a></td>
    <td>This paper introduces enhancements to LLaVA&#39;s architecture, employing a CLIP-ViT-L-336px vision encoder and an MLP projection layer, which significantly improves its data efficiency and performance across a range of benchmarks.</td>
    <td>The enhanced architecture includes the CLIP-ViT-L-336px for visual encoding and a multi-layer perceptron (MLP) for the vision-language cross-modal connector, enhancing the model&#39;s multimodal understanding.</td>
    <td>LLaVA-1.5 achieves state-of-the-art performance on 11 benchmarks with simple modifications, using a two-stage training approach focusing on efficient feature alignment and fine-tuning with academic-task-oriented VQA data.</td>
    <td>The paper focuses on improving multimodal alignment through instruction tuning, employing a more powerful MLP vision-language connector over the original linear projection, facilitating better integration of visual and linguistic data.</td>
    <td>Uses an MLP-based vision-language connector for more effective fusion of visual and textual representations, aligning them closely in the embedding space.</td>
    <td>VQA-v2, GQA, academic-task-oriented VQA datasets, incorporating OCR and region-level perception data.</td>
    <td>These datasets are used to significantly enhance the model&#39;s visual understanding and reasoning capabilities, demonstrating state-of-the-art performance with academic-task-oriented data.</td>
    </tr>
    </tbody>
    </table>
</details>


