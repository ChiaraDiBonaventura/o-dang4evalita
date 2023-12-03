# o-dang4evalita

Code for the paper "O-Dang at HODI and HaSpeeDe3: A Knowledge-Enhanced Approach to Homotransphobia and Hate Speech Detection in Italian", published in the Proceedings of the Eighth Evaluation Campaign of Natural Language Processing and Speech Tools for Italian. Final Workshop (EVALITA 2023), CEUR. org, Parma, Italy (https://ceur-ws.org/Vol-3473/paper29.pdf).

Shared tasks we partecipated in: 
* HaSpeeDe3: political and religious hate speech detection in Italian; 
* HODI: homotransphobia detection in Italian. 

The paper provides a simple, yet effective, approach to detect different types of hate speech in Italian (i.e., homotransphobia, political hate speech, religious hate speech) by leveraging Knowledge Graphs and LLMs prompting. Our knowledge-enhanced systems outperformed all the competition’s baselines. Our best submissions achieved the macro-F1 score of 0.912 for HaSpeeDe3 and 0.795 for HODI, reaching the 1st and 3rd place, respectively. 

### Repository description
The approach proposed in the paper is based on three steps: 1) Entity Linking (EL), 2) Knowledge Injection, and 3) Prediction. This 3-step approach is reflected in the structure of the repository: 

1. Entity Linking:
   * EL: contains information for the entity linking;
   * ontology: contains the ontology of dangerous speech messages, as introduced in Stranisci et al. (2022).
   
2. Knowledge Injection:
   * davinci002: contains the information retrieved when prompting text-davinci-002;
   * evalita: contains all the data needed to run the prediction for hate speech classification (haspeede) and homotransphobia (hodi).
   
3. Prediction:
   * HaSpeeDe.ipynb: contains the code for running the classification. 
