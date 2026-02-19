# 🎓 OpenResearch API

**One Request. Two Sources. Zero Parsing Hassle.**

Stop wasting time mapping different metadata schemas. **OpenResearch API** aggregates, normalizes, and deduplicates academic data from **OpenAlex** and **Crossref** into a single, clean JSON response.

[![RapidAPI](https://img.shields.io/badge/RapidAPI-Connect-blue?style=for-the-badge&logo=rapidapi)](https://rapidapi.com/fathoniadam933/api/openresearch-api)

---

### 🚀 Why Developers Love It
* **Unified Schema:** Crossref and OpenAlex data formatted identically. No more custom parsers.
* **Smart Deduplication:** Automatic DOI-based deduplication to keep your data clean.
* **Trend Insights:** Instant N-Gram analysis (unigrams, bigrams, trigrams) for topic exploration.
* **AI-Ready:** Perfect for feeding RAG pipelines, LLMs, or research dashboards.

### Available Endpoints 
| Endpoint | Method | Description |
|----------|--------|------------|
| /v1/papers/search | GET | Search papers by keyword with year filters. |
| /v1/papers/lookup | GET | Lookup paper metadata by DOI. |
| /v1/trends | GET | Get keyword publication trends and Analyze unigram/bigram/trigram trends from titles. |

### ⚡ Quick Start (cURL)
Get paper metadata in seconds:
```bash
curl --request GET \
  --url 'https://openresearch-api.p.rapidapi.com/v1/papers/search?query=machine%20learning&from_year=2020&to_year=2025&limit=10' \
  --header 'X-RapidAPI-Key: YOUR_RAPIDAPI_KEY' \
  --header 'X-RapidAPI-Host: openresearch-api.p.rapidapi.com'
```
To try this API, you can start with the Free plan on RapidAPI.

1. Open the OpenResearch API page on RapidAPI (link page below).

2. Subscribe using the Free plan (no payment needed).

3. Once subscribed, RapidAPI will automatically provide you with:

  - X-RapidAPI-Key
  
  - X-RapidAPI-Host

You can find both values directly in the Code Snippets or Headers section inside the RapidAPI dashboard.

Replace YOUR_RAPIDAPI_KEY in the example above with your actual key, and you’re good to go 🚀

The Free plan is intended for:

- Testing the API

- Exploring response formats

- Evaluating whether the data fits your use case

If the API works well for your project or production needs, you can easily upgrade to a higher plan (Pro / Ultra / Mega) to get higher rate limits and monthly quotas—no code changes required.

### 📦 Example Response

```
{
  "query": "machine learning",
  "filters": {
    "from_year": 2020,
    "to_year": 2025
  },
  "count": 10,
  "results": [
    {
      "title": "Physics-informed machine learning",
      "authors": [
        "George Em Karniadakis",
        "Ioannis G. Kevrekidis",
        "Lu Lu",
        "Paris Perdikaris",
        "Sifan Wang",
        "Liu Yang"
      ],
      "year": 2021,
      "doi": "https://doi.org/10.1038/s42254-021-00314-5"
    },
    {
      "title": "Machine Learning: Algorithms, Real-World Applications and Research Directions",
      "authors": [
        "Iqbal H. Sarker"
      ],
      "year": 2021,
      "doi": "https://doi.org/10.1007/s42979-021-00592-x"
    },
    {
      "title": "Machine learning and deep learning",
      "authors": [
        "Christian Janiesch",
        "Patrick Zschech",
        "Kai Heinrich"
      ],
      "year": 2021,
      "doi": "https://doi.org/10.1007/s12525-021-00475-2"
    },
    {
      "title": "Machine Learning Algorithms - A Review",
      "authors": [
        "Batta Mahesh"
      ],
      "year": 2020,
      "doi": "https://doi.org/10.21275/art20203995"
    },
    {
      "title": "On hyperparameter optimization of machine learning algorithms: Theory and practice",
      "authors": [
        "Li Yang",
        "Abdallah Shami"
      ],
      "year": 2020,
      "doi": "https://doi.org/10.1016/j.neucom.2020.07.061"
    },
    {
      "title": "Optimization and Machine Learning",
      "authors": [],
      "year": 2022,
      "doi": "https://doi.org/10.1002/9781119902881"
    },
    {
      "title": "Why Use Automated Machine Learning?",
      "authors": [
        "Kai R. Larsen",
        "Daniel S. Becker"
      ],
      "year": 2021,
      "doi": "https://doi.org/10.1093/oso/9780190941659.003.0001"
    },
    {
      "title": "Front Matter",
      "authors": [],
      "year": 2022,
      "doi": "https://doi.org/10.1002/9781119902881.fmatter"
    },
    {
      "title": "Index",
      "authors": [],
      "year": 2022,
      "doi": "https://doi.org/10.1002/9781119902881.index"
    },
    {
      "title": "Machine learning vs. neutrosophic machine learning",
      "authors": [
        "Shabbir Hassan"
      ],
      "year": 2025,
      "doi": "https://doi.org/10.1201/9781003606055-5"
    }
  ]
}
```

💳 Subscription Plans

OpenResearch API is available through RapidAPI subscription plans.

You can start with the Free plan to explore the API and test basic functionality.
Once you’re confident it fits your use case, upgrading to a higher plan is seamless and does not require any code changes.

Typical plan structure:

| Plan | Requests Quota | Rate Limit | Price |
| --- | --- | --- | --- |
| Free (Basic) | 1.000/month | 5/sec | $0 |
| Pro | 20.000/month | 80/min | $10/month |
| Ultra | 50.000/month | 120/min | $20/month |
| Mega | 200.000/month | 300/min | $50/month |

All plans include:

- Unified access to OpenAlex and Crossref data

- Clean, normalized responses

- Simple GET-based endpoints

You can manage or upgrade your plan anytime from the RapidAPI dashboard.

### Use Cases
- 🧠 AI builders doing data enrichment.

- 📚 Research tools and academic platforms.

- 🚀 Startups building discovery, analysis, or reference features.

- 🔧 Developers who want quick access to paper metadata without managing multiple APIs.

###  🚦 Rate Limits & Pricing
Rate limits depend on your subscription plan. Check our Pricing Page on RapidAPI for more details.

### 🚀 Try It on RapidAPI

Access the full documentation and subscribe here:

👉 [https://rapidapi.com/fathoniadam933/api/openresearch-api]
