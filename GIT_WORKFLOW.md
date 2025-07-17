# 📘 Git Çalışma Akışı – Kudüs Hilali Web Sitesi

Bu belge, Kudüs Hilali projesinde iki geliştiricinin birlikte sağlıklı ve düzenli şekilde çalışmasını sağlar.

---

## 🧑‍💻 Katılımcılar

- **Katılımcı:** @aliHimeyda  
- **Katılımcı:** @AhmetKattaa

---

## 📦 Repo Klonlama (İlk Kez)

```bash
git clone https://github.com/AhmetKattaa/kudus-hilali-site/
cd kudus-hilali-site
```

---

## 🌱 Yeni Özellik Geliştirirken Branch Aç

```bash
git checkout -b about
```

📌 Branch isimlendirme örnekleri:

- `homepage`
- `navbar`
- `footer-logo`
- `login-error`

---

## 💾 Değişiklikleri Kaydet (Commit)

```bash
git add .
git commit -m "Anasayfa tasarımı eklendi"
```

---

## 🚀 Uzak Repo’ya Gönder (Push)

```bash
git push origin feature/ozellik-adi
```

---

## 🔀 Pull Request (PR) Oluşturma

1. GitHub'a gir
2. "Compare & pull request" butonuna tıkla
3. Açıklama yaz ve gönder
4. Diğer geliştirici kodu gözden geçirip `main` branch’e merge eder

> ⚠️ Ana branch (`main`) üzerine doğrudan commit atmayın.

---

## 🔄 Her Sabah / Çalışmaya Başlamadan Önce

```bash
git checkout main
git pull origin main
```

---

## 🧹 Merge Sonrası Temizlik (Opsiyonel ama önerilir)

```bash
git branch -d feature/ozellik-adi                 # Lokal branch silinir
git push origin --delete feature/ozellik-adi      # Remote branch silinir
```

---

## ✅ Kurallar ve Notlar

- `main` dalı sadece test edilmiş, çalışan kodları içerir.
- Her yeni özellik için yeni bir branch açılır.
- Kod inceleme (review) yapılmadan merge yapılmaz.
- Commit mesajları kısa ve açıklayıcı olmalıdır.
- Günde 1 kez `main` güncellenmeli (`git pull`).

---

## 📁 Klasör Yapısı (Özet)

```
kudus-hilali-site/
├── backend/       ← PHP + MySQL (api, config, uploads)
└── frontend/      ← React.js + Bootstrap + Axios
```

---

🕊️ *"Temiz bir repo, huzurlu bir geliştirici demektir."*
