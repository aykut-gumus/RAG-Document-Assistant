# 📚 RAG Tabanlı Doküman Asistanı

Bu proje, bir kullanım kılavuzu üzerinden çalışan **Retrieval-Augmented Generation (RAG)** tabanlı bir doküman soru-cevap sistemi geliştirilmesini amaçlamaktadır.

Proje kapsamında **Arzum Chefy AR1139-B / AR1139-S El Blender Kullanma Kılavuzu** doküman olarak kullanılmıştır.

Sistem, kullanıcı tarafından sorulan soruya önce doküman içerisinden ilgili bilgileri getirerek, ardından bu bilgiler doğrultusunda cevap üretmektedir. Böylece modelin dokümanda bulunmayan bilgileri uydurma (hallucination) ihtimalinin azaltılması hedeflenmiştir.

---

## 🎯 Projenin Amacı

Bu çalışmada aşağıdaki RAG bileşenlerinin uygulanması amaçlanmıştır:

- PDF dokümanının yüklenmesi ve işlenmesi
- LangChain `Document` yapısının kullanılması
- Metadata oluşturulması
- Metin parçalama (chunking)
- Embedding oluşturulması
- Chroma vektör veritabanı kullanılması
- Cosine similarity ile retrieval
- Metadata filtreleme
- Similarity Search
- MMR (Maximal Marginal Relevance)
- Similarity Score Threshold
- LCEL ile RAG pipeline oluşturulması
- Kaynak ve sayfa bilgisi ile cevap üretimi
- `@tool` kullanımı
- Yapılandırılmış CSV verisinin ayrı bir tool üzerinden sorgulanması
- RAG öncesi ve sonrası sonuçların karşılaştırılması

---

## 🧠 Kullanılan Teknolojiler

| Teknoloji | Kullanım Amacı |
|---|---|
| Python | Projenin geliştirilmesi |
| Google Colab | Çalışma ortamı |
| Gemini 2.5 Flash | Cevap üretimi |
| LangChain | RAG pipeline ve doküman işlemleri |
| Sentence Transformers | Embedding oluşturma |
| Chroma | Vektör veritabanı |
| PyPDF | PDF metin çıkarma |
| Pandas | CSV veri işlemleri |
| LCEL | RAG pipeline oluşturma |

### Kullanılan Model

```text
google/gemini-2.5-flash
