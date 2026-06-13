# PubMed

NCBI PubMed is the primary biomedical literature database providing free access to over 35 million citations and abstracts from life science journals and online books. The Entrez Programming Utilities (E-utilities) REST API enables programmatic searching, retrieval, and linking of citations, article metadata, abstracts, full-text links, and MeSH terms across PubMed and 38 other NCBI databases.

**Human URL:** https://pubmed.ncbi.nlm.nih.gov/  
**Developer Portal:** https://www.ncbi.nlm.nih.gov/home/develop/api/  
**Base URL:** https://eutils.ncbi.nlm.nih.gov/entrez/eutils/  
**Operated by:** U.S. National Library of Medicine (NLM) / National Institutes of Health (NIH)

## APIs

| API | Base URL | Description |
|-----|----------|-------------|
| Entrez E-utilities | https://eutils.ncbi.nlm.nih.gov/entrez/eutils/ | Search, fetch, link, and summarize records across 38 NCBI databases |
| PMC OA API | https://www.ncbi.nlm.nih.gov/pmc/utils/oa/oa.fcgi | Citation data and download links for Open Access articles |
| PMC OAI-PMH | https://pmc.ncbi.nlm.nih.gov/api/oai/v1/mh/ | Metadata harvesting for all PMC archive items |
| PMC BioC API | https://www.ncbi.nlm.nih.gov/research/bionlp/RESTful/pmcoa.cgi | Full text in BioC XML/JSON for NLP and text mining |
| PMC ID Converter | https://pmc.ncbi.nlm.nih.gov/tools/idconv/api/v1/articles/ | Convert between PMID, PMCID, DOI, and manuscript IDs |

## E-utility Endpoints

| Endpoint | URL | Function |
|----------|-----|----------|
| ESearch | esearch.fcgi | Text search returning matching UIDs |
| ESummary | esummary.fcgi | Document summaries for a list of UIDs |
| EFetch | efetch.fcgi | Full formatted records (abstracts, XML, etc.) |
| EPost | epost.fcgi | Upload UIDs to History Server |
| ELink | elink.fcgi | Find linked records across databases |
| EInfo | einfo.fcgi | Database statistics and searchable fields |
| EGQuery | egquery.fcgi | Search all 38 databases simultaneously |
| ESpell | espell.fcgi | Spelling suggestions for search terms |
| ECitMatch | ecitmatch.cgi | Batch PubMed ID lookup from citation strings |

## Authentication

- **No API key:** 3 requests/second (free, no registration)
- **With API key:** 10 requests/second (free NCBI account required)

Obtain an API key at: https://account.ncbi.nlm.nih.gov/ (Settings page)

Include `api_key=YOUR_KEY` as a query parameter.

## Pricing

All NCBI/PubMed APIs are **free of charge** — operated as a public service by the U.S. National Library of Medicine.

## Links

- [Documentation](https://www.ncbi.nlm.nih.gov/books/NBK25497/)
- [Quick Start Guide](https://www.ncbi.nlm.nih.gov/books/NBK25500/)
- [PMC Developer Tools](https://pmc.ncbi.nlm.nih.gov/tools/developers/)
- [Support](https://support.nlm.nih.gov/)
- [Usage Policies](https://www.ncbi.nlm.nih.gov/home/about/policies/)
