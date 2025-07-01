# Coursera: Machine Learning Modeling Pipelines in Production (by DeepLearning.AI)

## About the repo
This repository contains materials in the Coursera course "Machine Learning Modeling Pipelines in Production," the third course in the Machine Learning Engineering for Production (MLOps) Specialization Certificate of DeepLearning.AI. This repository is mainly for reference. 

> Note: Some activities are not copied as those are done in Google Cloud.

## About the directories
* <b>```Week1```</b> is about neural architecture search; that is, how to effectively search for the best model that will scale for various serving needs while constraining model complexity and hardware requirements (specifically, Keras Tuner and AutoML are central to the labs)
* <b>```Week2```</b> is about model resource management techniques; that is, how to optimize and manage the compute, storage, and I/O resources your model needs in production environments during its entire lifecycle (specifically, dimensionality reduction, quantization, and pruning are central to the labs)
* <b>```Week3```</b> is about high-performance modelling; that is, distributed processing and parallelism techniques are implemented to make the most of the computational resources for training models efficiently (specifically, distributed training and knowledge distillation are central to the labs)
* <b>```Week4```</b> is about model analysis to debug and remediate the model and measure robustness, fairness, and stability (specifically, TensorBoard, TensorFlow Model Analysis, fairness indicators, and continuous evaluation and monitoring are central to the labs)
* <b>```Week5```</b> is all about model interpretability - the key to explaining the model’s inner workings to laypeople and expert audiences and how it promotes fairness and helps address regulatory and legal requirements for different use cases (specifically, permutation feature importance and SHAP are central to the labs)

## Reading/Video Links
The following are the reading/video links provided in each week of the course (copied here for future reference).

<b>Week 1: Neural Architecture Search</b>
* <a href="https://arxiv.org/pdf/1808.05377.pdf">Neural Architecture Search</a>
* <a href="https://distill.pub/2020/bayesian-optimization/">Bayesian Optimization</a>
* <a href="https://arxiv.org/pdf/1611.01578.pdf">Neural Architecture Search with Reinforcement Learning</a>
* <a href="https://arxiv.org/pdf/1712.00559.pdf">Progressive Neural Architecture Search</a>
* <a href="https://arxiv.org/abs/1603.01670">Network Morphism</a>
* <a href="https://aws.amazon.com/sagemaker/autopilot">Amazon SageMaker Autopilot</a>
* <a href="https://azure.microsoft.com/en-in/services/machine-learning/automatedml/">Microsoft Azure Automated Machine Learning</a>
* <a href="https://cloud.google.com/automl">Google Cloud AutoML</a>

<b>Week 2: Model Resource Management Techniques</b>
* <a href="https://heartbeat.fritz.ai/coreml-with-glove-word-embedding-and-recursive-neural-network-part-2-d72c1a66b028">Word embeddings</a>
* Curse of dimensionality:
  * https://builtin.com/data-science/curse-dimensionality</li>
  * https://www.visiondummy.com/2014/04/curse-dimensionality-affect-classification/</li>
* <a href="https://www.kdd.org/exploration_files/parsons.pdf">Sparsity</a>
* Feature engineering:
  * https://quantdare.com/what-is-the-difference-between-feature-extraction-and-feature-selection/
  * https://machinelearningmastery.com/discover-feature-engineering-how-to-engineer-features-and-how-to-get-good-at-it/
* Principal Component Analysis (PCA):
  * https://arxiv.org/pdf/1404.1100.pdf
  * https://scikit-learn.org/stable/modules/decomposition.html
  * https://www.coursera.org/lecture/machine-learning/principal-component-analysis-problem-formulation-GBFTt
  * https://stats.stackexchange.com/questions/2691/making-sense-of-principal-component-analysis-eigenvectors-eigenvalues/140579#140579
  * https://elitedatascience.com/dimensionality-reduction-algorithms
* Independent Component Analysis (ICA):
  * https://arxiv.org/pdf/1404.2986.pdf
  * https://scikit-learn.org/stable/modules/decomposition.html
  * https://scikit-learn.org/stable/auto_examples/decomposition/plot_ica_vs_pca.html
* <a href="https://scikit-learn.org/stable/modules/decomposition.html#non-negative-matrix-factorization-nmf-or-nnmf">NMF</a>
* <a href="http://alexhwilliams.info/itsneuronalblog/2016/03/27/pca/">PCA extensions</a>
* Mobile model deployment:
  * https://developers.google.com/ml-kit
  * https://www.tensorflow.org/lite
* Quantization:
  * https://arxiv.org/abs/1712.05877</li>
  * https://www.qualcomm.com/news/onq/2019/03/12/heres-why-quantization-matters-ai
  * https://petewarden.com/2016/05/03/how-to-quantize-neural-networks-with-tensorflow/
  * https://blog.tensorflow.org/2020/04/quantization-aware-training-with-tensorflow-model-optimization-toolkit.html
  * https://www.tensorflow.org/lite/performance/best_practices</li>
* <a href="https://medium.com/tensorflow/introducing-the-model-optimization-toolkit-for-tensorflow-254aca1ba0a3">Post-training quantization</a>
* <a href="https://blog.tensorflow.org/2020/04/quantization-aware-training-with-tensorflow-model-optimization-toolkit.html">Quantization aware training</a>
* Pruning:
  * https://proceedings.neurips.cc/paper/1989/file/6c9882bbac1c7093bd25041881277658-Paper.pdf
  * https://blog.tensorflow.org/2019/05/tf-model-optimization-toolkit-pruning-API.html
  * http://yann.lecun.com/exdb/publis/pdf/lecun-90b.pdf
  * https://towardsdatascience.com/can-you-remove-99-of-a-neural-network-without-losing-accuracy-915b1fab873b
  * https://arxiv.org/abs/1803.03635
  * https://numenta.com/blog/2019/08/30/case-for-sparsity-in-neural-networks-part-1-pruning
  * https://www.tensorflow.org/model_optimization/guide/pruning
* <a href="https://arxiv.org/abs/1803.03635">The Lottery Ticket Hypothesis</a>

<b>Week 3: High-Performance Modeling</b>
* <a href="https://www.tensorflow.org/guide/distributed_training">Distributed training</a>
* <a href="https://arxiv.org/abs/1806.03377">Data parallelism</a>
* <a href="https://ai.googleblog.com/2019/03/introducing-gpipe-open-source-library.html">Pipeline parallelism</a>
* <a href="https://arxiv.org/abs/1811.06965">GPipe</a>
* <a href="https://arxiv.org/abs/1409.4842">GoogleNet</a>
* Knowledge distillation:
  * https://arxiv.org/pdf/1503.02531.pdf
  * https://ai.googleblog.com/2018/05/custom-on-device-ml-models.html
  * https://nervanasystems.github.io/distiller/knowledge_distillation.html
* <a href="https://blog.tensorflow.org/2020/05/how-hugging-face-achieved-2x-performance-boost-question-answering.html">DistilBERT</a>
* <a href="https://arxiv.org/pdf/1910.08381.pdf">Two-stage multi-teacher distillation for Q&A case study</a>
* <a href="https://arxiv.org/abs/1911.04252">EfficientNets</a>

<b>Week 4: Model Analysis</b>
* <a href="https://blog.tensorflow.org/2019/12/introducing-tensorboarddev-new-way-to.html">TensorBoard</a>
* <a href="https://www.kaggle.com/c/dogs-vs-cats/data">Model Introspection</a>
* <a href="https://cs231n.github.io/neural-networks-3/">Optimization process</a>
* <a href="https://blog.tensorflow.org/2018/03/introducing-tensorflow-model-analysis.html">TFMA</a>
* <a href="https://www.tensorflow.org/tfx/model_analysis/architecture">TFMA architecture</a>
* <a href="https://blog.tensorflow.org/2018/03/introducing-tensorflow-model-analysis.html">Aggregate versus slice metrics</a>
* What-if tool:
  * https://pair-code.github.io/what-if-tool/
  * https://www.youtube.com/playlist?list=PLIivdWyY5sqK7Z5A2-sftWLlbVSXuyclr
* <a href="https://arxiv.org/abs/1412.6572">Explaining and Harnessing Adversarial Examples</a>
* <a href="https://github.com/SauceCat/PDPbox">PDPbox</a> and <a href="https://github.com/AustinRochford/PyCEbox">PyCEbox</a>
* Adversarial attacks:
  * http://karpathy.github.io/2015/03/30/breaking-convnets/
  * https://arxiv.org/pdf/1707.08945.pdf
* <a href="https://fpf.org/wp-content/uploads/2019/09/FPF_WarningSigns_Report.pdf">Informational and behavioral harms</a>
* <a href="https://github.com/cleverhans-lab/cleverhans">Clever Hans</a>
* <a href="https://foolbox.jonasrauber.de/">Foolbox</a>
* <a href="https://arxiv.org/abs/1511.04508">Defensive distillation</a>
* <a href="https://www.tensorflow.org/responsible_ai/fairness_indicators/guide">Fairness</a>
* <a href="https://arxiv.org/pdf/1904.13341.pdf">Learning fair representations</a>
* <a href="https://github.com/cosmicBboy/themis-ml">Fairness-aware Machine Learning library</a>
* <a href="https://www.tensorflow.org/responsible_ai/model_remediation">Model remediation</a>
* <a href="http://aif360.mybluemix.net/">AIF360</a>
* <a href="https://github.com/cosmicBboy/themis-ml">Themis ML</a>
* <a href="https://arxiv.org/pdf/1904.13341.pdf">LFR</a>
* <a href="https://modelcards.withgoogle.com/about">Model cards</a>
* <a href="https://www.infoq.com/presentations/instrumentation-observability-monitoring-ml/">Instrumentation, Observability & Monitoring of Machine Learning Models</a>
* <a href="https://christophergs.com/machine%20learning/2020/03/14/how-to-monitor-machine-learning-models/">Monitoring Machine Learning Models in Production - A Comprehensive Guide</a>
* <a href="https://arxiv.org/pdf/1704.00023.pdf">Concept Drift detection for Unsupervised Learning</a>
* <a href="https://cloud.google.com/ai-platform/prediction/docs/continuous-evaluation">Google Cloud</a>
* <a href="https://aws.amazon.com/sagemaker/model-monitor/">Amazon SageMaker</a>
* <a href="https://docs.microsoft.com/en-us/azure/machine-learning/how-to-monitor-datasets">Microsoft Azure</a>

<b>Week 5: Interpretability</b>
* Fooling DNNs:
  * https://arxiv.org/pdf/1607.02533.pdf
  * https://arxiv.org/pdf/1412.6572.pdf
* <a href="http://www.cs.columbia.edu/~orb/papers/xai_survey_paper_2017.pdf">XAI</a>
* <a href="https://ojs.aaai.org/index.php/aimagazine/article/view/2850/3419">Explainable AI</a>
* <a href="https://arxiv.org/pdf/1910.10045.pdf">Responsible AI</a>
* <a href="https://christophm.github.io/interpretable-ml-book/">Interpretable Machine Learning - A Guide for Making Black Box Models Explainable</a>
* <a href="https://en.wikipedia.org/wiki/Dolbear%27s_law">Dolbear's Law</a>
* TensorFlow Lattice:
  * https://www.tensorflow.org/lattice
  * https://jmlr.org/papers/volume17/15-243/15-243.pdf
* <a href="https://scikit-learn.org/stable/auto_examples/inspection/plot_partial_dependence.html">PDP</a>
* <a href="https://jmlr.org/papers/volume17/15-243/15-243.pdf">Monotonic Calibrated Interpolated Look-Up Tables</a>
* <a href="http://arxiv.org/abs/1801.01489">Permutation feature importance</a>
* <a href="https://en.wikipedia.org/wiki/Shapley_value">Shapley values</a>
* <a href="https://github.com/slundberg/shap">SHAP</a>
* <a href="https://proceedings.neurips.cc/paper/2017/file/8a20a8621978632d76c43dfd28b67767-Paper.pdf">A Unified Approach to Interpreting Model Predictions</a>
* <a href="https://arxiv.org/abs/1905.04610">Explainable AI for Trees: From Local Explanations to Global Understanding</a>
* <a href="https://arxiv.org/pdf/1711.11279.pdf">TCAV</a> and <a href="https://github.com/marcotcr/lime">LIME</a>
* <a href="https://storage.googleapis.com/cloud-ai-whitepapers/AI%20Explainability%20Whitepaper.pdf">Google Cloud XAI / AI Explanations</a>
* <a href="https://arxiv.org/pdf/1703.01365.pdf">Integrated gradients</a>

## Aditional overall resources
* <a href="https://arxiv.org/abs/2010.02013">Towards ML Engineering - History of TFX</a>
* <a href="https://arxiv.org/abs/2011.09926">Challenges in Deploying ML</a>
