# Arabic_classification_transformer
1. Bidirectional LSTM 
2. Logical AraVec Validation (Word Similarity + Vector Math) 
3.  Shows Raw &amp; Cleaned Data
4.  90-10 Train-Test Split 
5. Preprocessing, Tokenization &amp; Padding 
6. Confusion Matrix + Classification Report 
7. Train &amp; Validation Loss Curve 
8. Testing on New Arabic Sentences 
9.  Final Summary &amp; Insights


# Best Results 
1. Model 3 
![WhatsApp Image 2025-03-17 at 22 56 21_8ba3bf79](https://github.com/user-attachments/assets/e4b161d0-178f-4434-b42c-41d46adc5d58)

2. Model 4
![image](https://github.com/user-attachments/assets/37761dde-3923-4ef4-96f8-f7b75e351720)

3. Model 2
![image](https://github.com/user-attachments/assets/71088259-5d0d-4222-b9bd-3afc3da06375)

4. Model 1
![image](https://github.com/user-attachments/assets/5c59f0dc-28e9-441f-b3ae-a50506b1fc44)

I realized that all these extra layers and tweaks just slowed things down. The simple LSTM setup works best for me — clean, efficient, and fast enough without overkill.

#overal trials
Original model: 2 Bidirectional LSTM layers (128 & 64), dropout, simple and balanced.
First modification: Switched to GRU, added GlobalMaxPooling1D, Dense(64), and recurrent dropout.
Second modification: Enabled mixed precision, used learning rate scheduler — became too heavy and slow.
final change was the number of epoch from 10 - 6 , using cross validation
