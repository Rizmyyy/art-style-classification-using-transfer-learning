# art-style-classification-using-transfer-learning
Sistem klasifikasi gaya seni lukisan menggunakan Artificial Neural Network (ANN). Proyek ini mencakup preprocessing dataset, pelatihan model, evaluasi menggunakan confusion matrix &amp; ROC curve, serta notebook lengkap yang dapat dijalankan di Google Colab.
Model dapat mengklasifikasikan 4 gaya seni:
• Abstract Expressionism
• Cubism
• Early Renaissance
• Ukiyo-e

# 📌 Fitur Utama
• Menggunakan MobileNetV2 sebagai feature extractor.
• ANN head untuk klasifikasi (Dense → Dropout → Dense).
• Augmentasi data untuk mencegah overfitting.
• Confusion Matrix, ROC Curve, Precision/Recall/F1.
• Prediksi gambar upload di Google Colab.

# 🧠 Arsitektur Model
• Input: 224×224 RGB
• Feature extractor: MobileNetV2 (pretrained ImageNet)
• ANN classifier:
  • Dense(256) + ReLU + Dropout
  • Dense(128) + ReLU + Dropout
  • Dense(4) + Softmax

# 📚 Dataset
Dataset terdiri dari 4 kelas, masing-masing dipecah menjadi:
• subset_train/ → untuk training dan validation
• subset_test/ → untuk evaluasi akhir
dataset bisa didownload di folder dataset dalam bentuk zip lalu diekstrak dan diupload ke google drive pribadi.
