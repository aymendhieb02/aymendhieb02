# Selected engineering work

A closer look at my contributions, methods and project status.

## BCMID — Multimodal RAG and agents

**Problem.** Explore breast-imaging reports, similar training images and structured metadata while keeping answers tied to their sources.

**My contribution.** Implemented n8n-to-FastAPI tool workflows and the Streamlit research interface; worked across retrieval and data preparation within the group project.

**Methods.** Multilingual E5 embeddings, BM25/RRF hybrid retrieval, ChromaDB, local Ollama inference and seven agent roles: an orchestrator, four retrieval specialists, an evidence checker and a response generator. Patient-level preparation keeps training and evaluation records separate.

**Status.** Research prototype. The public n8n export is an inactive import template, and the canvas is architecture evidence. Runtime verification depends on the workflow revision and local services. The system retrieves and attributes evidence; it does not diagnose.

[Repository and architecture](https://github.com/aymendhieb02/bcmid) · [Verification notes](https://github.com/aymendhieb02/bcmid/blob/main/docs/verification-status.md)

## DressMe — Garment classification and virtual try-on

**Problem.** Turn garment photos into a reviewed digital wardrobe entry and investigate pretrained virtual try-on models.

**My contribution.** Worked on BO6 wardrobe digitization and BO7 virtual try-on in the six-person team, including classification/model evaluation and pretrained-model notebook experiments.

**Methods.** An 11-class EfficientNet-B0 classifier, transfer learning, eligible attribute heads, structured descriptions and user review. BO7 experiments cover FASHN VTON and CatVTON separately from the classification service.

**Evaluation.** The exported classifier reports macro-F1 **0.8882** and accuracy **0.9316** on **2,310 catalog validation images**. The reserved test split has not been run, and real phone-photo performance has not been measured. Exact duplicate checks and the remaining near-duplicate risks are documented in the model card. The result is validation performance for this export.

[Repository](https://github.com/aymendhieb02/DressMe) · [Model card](https://github.com/aymendhieb02/DressMe/blob/main/ml-service/bundle/model_card.md) · [Validation metrics](https://github.com/aymendhieb02/DressMe/blob/main/ml-service/bundle/validation_metrics.json)

## Smart OCR-to-ERP — Invoice document intelligence

**Problem.** Convert invoice PDFs/scans into reviewable fields, line items and ERP-oriented JSON.

**My contribution.** Independently developed OCR/extraction pipelines and delivered client-specific Docker APIs. The client workflows include structured extraction, financial validation and review/correction.

**Methods.** Native PDF text when available, PaddleOCR/OpenCV processing, candidate extraction, evidence and deterministic business checks, exposed through FastAPI.

**Status.** Client Docker handovers are separate from the public development build. The repository explains which source, Dockerfile and release artifacts correspond to which scope; the root development build does not reproduce every delivered image exactly.

[Repository and release boundaries](https://github.com/aymendhieb02/Smart-OCR-to-ERP-Platform)

## Tender Document Intelligence — Requirements and BOQ

**Problem.** Help reviewers inspect requirements, evidence and pricing information in tender documents.

**My contribution.** Independently built the core during the internship and continued improving and validating it with a client contact.

**Methods.** A reusable PDF/OCR evidence layer, source-linked requirements, lexical question answering, and template-specific BOQ/pricing export.

**Status.** Evaluated on seven development documents; client validation continues. The lexical question-answering path is distinct from an LLM-based RAG system.

[Repository and technical documentation](https://github.com/aymendhieb02/tender-document-intelligence)

## Ask Your Document — Conversational document retrieval

**Problem.** Ask questions about an uploaded text document and inspect the supporting sources.

**My contribution.** Built the document assistant as a hackathon product. Other hackathon products in the repository are separate workstreams.

**Methods.** Text chunking, embeddings, ChromaDB retrieval, LLM-provider integration, citations and conversational history in a Streamlit interface. MongoDB supports the history layer.

**Status.** Hackathon prototype. The current uploader accepts `.txt` files; broader document-format support is not implied.

[Project overview](https://github.com/aymendhieb02/onyX) · [Application source](https://github.com/aymendhieb02/onyX/tree/Ask_Your_Document/AskYourDocument)

## Stroke Prediction — Imbalanced tabular classification

**Problem.** Compare models on a small, strongly imbalanced classification dataset in a competition setting.

**My contribution.** Handled the data/modeling workflow and application components within team OnyX.

**Methods.** Data inspection, missing-value treatment, encoding, feature engineering, model comparison and ROC-AUC evaluation, with Flask/Streamlit demonstration interfaces.

**Status.** Competition and educational prototype, not a clinically validated prediction system. A public leaderboard result should be distinguished from final competition standings and independent validation.

[Repository and notebooks](https://github.com/aymendhieb02/onyX_hackathon_mario_hack_Intelligent_Stroke_Prediction_System)
