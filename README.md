📰 Russian Text Classification (SIB-200)

MODEL USED 🤖
I fine-tuned ai-forever/ruRoberta-large, a STRONG transformer model built for the Russian language.

DATASET 📚
The model is trained and evaluated on SIB-200 (rus_Cyrl), a LARGE multilingual news classification dataset with 200 categories.

SMART TRAINING CHANGES ⚙️
Instead of increasing epochs, I improved results using class-weighted loss, label smoothing, gradient accumulation, and a LOWER learning rate with warmup.

RUNS ON FREE COLAB 💻
Training is optimized to run on the FREE Google Colab T4 GPU (15 GB RAM) by reducing batch size, freezing lower layers, and using FP16.

RESULTS & EVALUATION 📊
The best model is selected using MACRO F1-score, giving more balanced performance across all classes.
