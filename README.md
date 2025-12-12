# 🏛️ Chatbot RAG - Sites Archéologiques de Tunisie

## 📋 Description
Chatbot intelligent spécialisé sur l'archéologie tunisienne utilisant l'architecture RAG (Retrieval-Augmented Generation).  
Projet académique pour maîtriser le pipeline RAG complet.

## 🎯 Objectifs Pédagogiques
- Collecte et préparation de 50+ documents structurés
- Découpage sémantique et génération d'embeddings
- Indexation dans base vectorielle ChromaDB
- Pipeline RAG complet avec LLM local (Llama 2)
- Interface utilisateur avec Streamlit
- Évaluation de robustesse (10 questions testées)

## 🛠️ Technologies Utilisées
- **LLM** : Llama 2 via Ollama
- **Base vectorielle** : ChromaDB
- **Embeddings** : sentence-transformers/all-MiniLM-L6-v2
- **Interface** : Streamlit
- **Langages** : Python 3.11, Français/Anglais/Arabe

## 📁 Structure du Projet
tunisian-archaeology-rag/
├── data/ # Données
│ ├── raw_50/ # 50 documents sources
│ └── processed/ # Chunks prétraités
├── src/ # Code source
│ ├── chroma_manager.py # Gestion base vectorielle
│ ├── rag_pipeline.py # Pipeline RAG principal
│ ├── preprocessing.py # Prétraitement documents
│ ├── embedding.py # Génération embeddings
│ └── evaluation.py # Évaluation chatbot
├── app.py # Interface Streamlit
├── requirements.txt # Dépendances Python
├── LICENSE # Licence MIT
└── README.md # Ce fichier

## 🚀 Installation & Utilisation

### Prérequis
- Python 3.8+
- Ollama (https://ollama.com)
- 8GB RAM minimum

### Installation
```bash
# 1. Cloner le projet
git clone https://github.com/[username]/tunisian-archaeology-rag.git
cd tunisian-archaeology-rag

# 2. Installer les dépendances
pip install -r requirements.txt

# 3. Télécharger le modèle Llama 2
ollama pull llama2:latest

# 4. Lancer Ollama en arrière-plan
ollama serve
# Démarrer l'interface
streamlit run app.py

# Puis ouvrir http://localhost:8501


📊 Fonctionnalités
✅ Base de connaissances : 50+ documents sur 10 sites archéologiques

✅ Recherche sémantique avec similarité cosinus

✅ Génération de réponses factuelles avec sources citées

✅ Interface multilingue (français, anglais, arabe)

✅ Historique des conversations

✅ Scores de confiance calculés

✅ Évaluation robuste avec 10 questions testées


**Réponse** : [texte clair et précis]

**Sources** :
- [Titre document 1] (source: Wikipedia, site: Carthage)
- [Titre document 2] (source: UNESCO, site: Dougga)


🧪 Évaluation
10 questions testées avec métriques :

Score mots-clés : 78%

Pertinence sources (>0.7) : 71%

Absence d'hallucinations : 95%

Score global : 72%

👤 Auteur
Yosser Kallel - Projet académique IA Générative
