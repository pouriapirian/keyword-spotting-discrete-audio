# Keyword Spotting with Discrete Representations  

## Overview  
This project evaluates the performance of **discrete audio representations** for **keyword spotting (KWS)**.  
Traditional KWS methods rely on continuous features like **FBANKs, MFCCs, or self-supervised features** (e.g., Wav2Vec, HuBERT, WavLM).  
However, **discrete audio tokens** (such as those from Encodec and DAC) have gained interest due to their potential benefits, such as:  
- **Better integration** with large multimodal language models.  
- **Transforming regression problems into classification problems**, making them easier to handle.  

This project aims to compare the performance of **discrete representations** against **standard continuous features** and **self-supervised models** for keyword spotting.  

---

## Dataset  
We use the **Google Speech Commands Dataset**, a widely used dataset for KWS tasks.  
- **Dataset Link:** [Google Speech Commands](https://ai.googleblog.com/2017/08/launching-speech-commands-dataset.html)  
- Contains **short audio clips of spoken words** (e.g., "yes," "no," "left," "right").  

---

## Methodology  
1. **Literature Review**  
   - Research on existing discrete audio representation models (e.g., Encodec, DAC).  

2. **Data Preparation**  
   - Use the **Google Speech Commands Dataset**.  
   - Preprocess data for different feature extraction methods.  

3. **Feature Extraction & Model Training**  
   - Extract features using:  
     - **Discrete Representations** (e.g., Encodec, DAC).  
     - **Standard Features** (MFCCs, FBANKs).  
     - **Self-Supervised Models** (Wav2Vec, HuBERT, WavLM).  
   - Train keyword spotting models using SpeechBrain’s existing implementations.  

4. **Performance Comparison**  
   - Evaluate models based on accuracy and efficiency.  
   - Compare discrete representations against continuous features.  

---