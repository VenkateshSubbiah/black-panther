## Amazon Comprehend
This can analyse the documents and extract insights out of it using machine learning. It has inbuilt NLP capabilities and has a default model that's been trained on huge data. It keeps updating based on our data too.
- Insights
	- Entities
	- Key phrases
	- PII
	- Language - Has 'Dominant language' capability. Also supports many languages.
	- Sentiment
	- Targeted sentiment - Sentiment of entities
	- Syntax - parts of speech.
- Comprehend custom - Uses AutoML to build custom models for your requirements. Custom classification and custom entity recognition are possible.
- Flywheels - Orchestrates training and managing custom model versions.
- Document clustering (topic modelling) - Can group documents based on topics.

No provisioning required. Pay per request. Custom model training and storing is billed.
Synchronous mode can process 1 document or a batch of 25 documents.
Asynchronous job can process large number of documents.
## Amazon Forecast
Helps time-series forecasting using statistical and machine learning algorithms.
## Amazon Fraud Detector
Uses machine learning to detect fraudulent activities online. Data can be sent to the service which then creates custom model and also with the help of 20 years of fraud detection expertise at amazon. We can also configure decision logic of the model.
## Amazon Kendra
Intelligent search service that can return answers for questions by searching through the data or documents provided. It has NLP capabilities and has semantic and contextual understanding to find answers.
## Amazon Lex
Helps build conversational interfaces based on voice and text. It has Natural language understanding and Automatic Speech Recognition capabilities.
## Amazon Polly
Text to speech (TTS) engine. Uses deep learning to output life like voices. Supports,
- Various languages
- SSML - Speech Synthesis Markup Language - better control on the speech
	- Emphasis
	- Phonetic pronounciation
	- Breathing sounds
	- Whispering
	- Newscaster style
## Amazon Rekognition
Image and video analysis using ML. Features - object detection, text recognition, facial analysis, celebrity recognition, custom labels, unsafe content detection (content moderation). 
## Amazon SageMaker
Fully managed machine learning service. One can build and train models in Sagemaker without having to manually provision servers. Also this has distributed training options.
## Amazon Textract
Extracts text from documents (Images, PDF etc).
## Amazon Transcribe
Speech to text using deep learning. Audio can be streamed or can be stored in S3. 
Features - PII redaction, language identification for multi-lingual audio.
## Amazon Translate
Translates using machine learning.