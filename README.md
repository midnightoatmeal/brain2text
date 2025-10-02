# brain2text
Brain-to-Text AI is a Neuralink-inspired brain-computer interface that translates human brain activity into text using EEG (electroencephalography) signals. The project demonstrates how deep learning can be applied to noisy neural data, transforming raw brainwave activity into meaningful words and sentences.

(Currently at the MVP stage: preprocessing scripts and baseline models are under development)

## Features

    1. Data Collection
We use open-source EEG datasets where participants spoke or imagined words while their brain activity was recorded (e.g., PhysioNet EEG Speech, BCI Competition IV).

	2.	Signal Preprocessing
	Raw EEG is extremely noisy, so we clean and transform the data into usable features:
	•	Bandpass filtering and artifact removal.
	•	Spectrogram and Fourier transform representations.
	•	Normalization and alignment with text labels.
	
	3.	Deep Learning Models
	Multiple architectures are explored for mapping EEG → Text:
	•	CNN/LSTM hybrids for sequence modeling.
	•	Transformers (small GPT-like models) fine-tuned on EEG embeddings.
	•	Contrastive learning approaches (CLIP-style) pairing EEG with language embeddings.
	
	4.	Demo Application
	A simple Streamlit web app showcases the system:
	•	Upload EEG data and view predicted text outputs.
	•	Visualize brainwave activity in real time.
	•	Stretch goal: connect to a consumer EEG headset (Muse 2, OpenBCI) for real-time brain typing.

## Highlights
	•	End-to-end pipeline: raw EEG → cleaned signals → deep learning → text.
	•	Modular design for experimenting with different models and datasets.
	•	Interactive demo to make the research accessible.
