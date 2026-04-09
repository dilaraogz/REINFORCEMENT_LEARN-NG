# REINFORCEMENT_LEARN-NG# 🚕 Q-Learning Taxi Projesi (6x6 Grid)

Bu projede Reinforcement Learning (Pekiştirmeli Öğrenme) kullanılarak bir taksi problemi çözülmüştür.

## 📌 Proje Özeti

- Grid boyutu: 6x6
- Müşteri lokasyonu: 5 farklı nokta
- Amaç: Müşteriyi alıp doğru hedefe bırakmak

## 🧠 Kullanılan Yöntem

Bu projede **Q-Learning algoritması** kullanılmıştır.

Q-Learning, ajan'ın çevre ile etkileşime girerek en iyi aksiyonları öğrenmesini sağlar.

## ⚙️ Durum (State)

Her state şu bilgilerden oluşur:

- Taxi konumu (row, col)
- Müşteri konumu
- Hedef konum

## 🎮 Aksiyonlar

Toplam 6 aksiyon vardır:

- Yukarı
- Aşağı
- Sol
- Sağ
- Müşteri al (pickup)
- Müşteri bırak (dropoff)

## 🏆 Ödül Sistemi

- Her adım: -1
- Yanlış pickup/drop: -10
- Doğru teslim: +20

## 📉 Epsilon-Greedy Stratejisi

Başlangıçta ajan rastgele hareket eder (exploration).

Zamanla:
- epsilon azalır
- ajan öğrendiğini kullanır (exploitation)

## 📊 Sonuç

Eğitim sonrası ajan:
- En kısa yolu bulmayı öğrenir
- Hataları azaltır
- Başarıyla müşteriyi taşır
