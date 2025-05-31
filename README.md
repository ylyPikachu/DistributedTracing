# Distributed Tracing Literature Analysis - Reproducible Search Methodology

This repository contains the complete methodology and data for our systematic literature review on distributed tracing research trends (2020-2024).

## 🔍 Reproducible Search Examples

### Search Parameters Overview

**Keywords Used:** `"distributed tracing"` (exact phrase)  
**Time Period:** 2020-2024  
**Publishers:** IEEE Xplore, ACM Digital Library, Springer, Elsevier, MDPI  
**Initial Results:** 539 papers → 483 papers (after manual filtering)

---

## Publisher-Specific Search Examples

### 1. IEEE Xplore Search

**Search URL Example:**
```
[https://ieeexplore.ieee.org/search/searchresult.jsp?queryText="distributed tracing"&highlight=true&returnFacets=ALL&returnType=SEARCH&matchPubs=true&pageNumber=1&refinements=ContentType:Conferences&refinements=ContentType:Journals&refinements=PublicationYear:2020&refinements=PublicationYear:2021&refinements=PublicationYear:2022&refinements=PublicationYear:2023&refinements=PublicationYear:2024](https://ieeexplore.ieee.org/search/searchresult.jsp?queryText=%22distributed%20tracing%22&highlight=true&returnType=SEARCH&matchPubs=true&ranges=2020_2024_Year&returnFacets=ALL&rowsPerPage=75&pageNumber=1)
```

**Search Parameters:**
- **Query:** `"distributed tracing"` (with quotes for exact match)
- **Date Range:** 2020-2024
- **Advanced Filter:** Full text search enabled

**Result:**
```
Search Query: "distributed tracing"
Results: 53 papers
```

### 2. ACM Digital Library Search

**Search URL Example:**
```
[https://dl.acm.org/action/doSearch?fillQuickSearch=false&target=advanced&query=%22distributed+tracing%22&AfterYear=2020&BeforeYear=2024&ContentItemType=research-article&ContentItemType=review-article](https://dl-acm-org.offcampus.lib.washington.edu/action/doSearch?AllField=%22distributed+tracing%22&pageSize=50&startPage=&AfterYear=2020&BeforeYear=2024&queryID=52/9094273692)
```

**Search Parameters:**
- **Query:** `"distributed tracing"` (exact phrase)
- **Publication Date:** After 2020, Before 2025
- **Search Fields:** Anywhere in document

**Result:**
```
Search Query: "distributed tracing"
Results: 188 papers
```

### 3. Elsevier

**Search URL Example:**
```
[[https://dl.acm.org/action/doSearch?fillQuickSearch=false&target=advanced&query=%22distributed+tracing%22&AfterYear=2020&BeforeYear=2024&ContentItemType=research-article&ContentItemType=review-article](https://dl-acm-org.offcampus.lib.washington.edu/action/doSearch?AllField=%22distributed+tracing%22&pageSize=50&startPage=&AfterYear=2020&BeforeYear=2024&queryID=52/9094273692)](https://www.sciencedirect.com/search?qs=%22distributed%20tracing%22&years=2024%2C2023%2C2022%2C2021%2C2020&lastSelectedFacet=articleTypes&articleTypes=CH)
```

**Search Parameters:**
- **Query:** `"distributed tracing"` (exact phrase)
- **Publication Date:** After 2020, Before 2025
- **Search Fields:** Anywhere in document

**Result:**
```
Search Query: "distributed tracing"
Results: 41 papers
```

### 4. Springer Search

**Search URL Example:**
```
[https://link.springer.com/search?query=%22distributed+tracing%22&date-facet-mode=between&facet-start-year=2020&facet-end-year=2024&facet-content-type=%22Article%22&facet-content-type=%22ConferencePaper%22](https://link.springer.com/search?new-search=true&advancedSearch=true&sortBy=relevance&query=%22distributed+tracing%22&title=&contributor=&journal=&date=custom&dateFrom=2020&dateTo=2024)
```

**Search Parameters:**
- **Query:** `"distributed tracing"`
- **Date Range:** 2020-2024
- **Disciplines:** Computer Science (when available)

**Result:**
```
Search Query: "distributed tracing"
Date: 2024
Results: 172 papers
```
### 5. Wiley

**Search URL Example:**
```
[[https://dl.acm.org/action/doSearch?fillQuickSearch=false&target=advanced&query=%22distributed+tracing%22&AfterYear=2020&BeforeYear=2024&ContentItemType=research-article&ContentItemType=review-article](https://dl-acm-org.offcampus.lib.washington.edu/action/doSearch?AllField=%22distributed+tracing%22&pageSize=50&startPage=&AfterYear=2020&BeforeYear=2024&queryID=52/9094273692)](https://onlinelibrary.wiley.com/action/doSearch?AfterYear=2024&AllField=%22distributed+tracing%22&BeforeYear=2024&ConceptID=68&content=articlesChapters&field1=AllField&target=default&text1=%22distributed+tracing%22)
```

**Search Parameters:**
- **Query:** `"distributed tracing"` (exact phrase)
- **Publication Date:** From 2020 January, to 2024 December
- **Search Fields:** Computer Science

**Result:**
```
Search Query: "distributed tracing"
Results: 9 papers
```

### 5. MDPI

**Search URL Example:**
```
[[[https://dl.acm.org/action/doSearch?fillQuickSearch=false&target=advanced&query=%22distributed+tracing%22&AfterYear=2020&BeforeYear=2024&ContentItemType=research-article&ContentItemType=review-article](https://dl-acm-org.offcampus.lib.washington.edu/action/doSearch?AllField=%22distributed+tracing%22&pageSize=50&startPage=&AfterYear=2020&BeforeYear=2024&queryID=52/9094273692)](https://onlinelibrary.wiley.com/action/doSearch?AfterYear=2024&AllField=%22distributed+tracing%22&BeforeYear=2024&ConceptID=68&content=articlesChapters&field1=AllField&target=default&text1=%22distributed+tracing%22)](https://www.mdpi.com/search?sort=pubdate&page_count=50&q=%22distributed+tracing%22&year_from=2020&year_to=2024&featured=&subjects=&journals=&article_types=&countries=)
```

**Search Parameters:**
- **Query:** `"distributed tracing"` (exact phrase)
- **Publication Date:** Between: 2020 - 2024
- **Search Fields:** Computer Science & Mathematics (8)

**Result:**
```
Search Query: "distributed tracing"
Results: 58 papers
Applied Search Fields: Computer Science & Mathematics: 8 papers
Manual Filter: 5 papers
```
---

## Search Execution Workflow

### Step-by-Step Process

1. **Navigate to Publisher Search Interface**

2. **Configure Search Parameters**
   ```
   Search Term: "distributed tracing" (with quotes)
   Search Fields: Document Title, Abstract, Index Terms
   Publication Years: 2020, 2021, 2022, 2023, 2024
   Content Types: Conferences, Journals, Magazines
   ```

3. **Execute Year-by-Year Searches**
   ```python
   # Example search parameters for automation
   years = ['2020', '2021', '2022', '2023', '2024']
   query = '"distributed tracing"'
   
   for year in years:
       search_params = {
           'query': query,
           'year': year,
           'content_types': ['conferences', 'journals']
       }
       # Execute search and record results
   ```

4. **Record Raw Results**

---

## Manual Filtering Examples

### Inclusion Criteria
✅ **Include:** Papers focusing on:
- Distributed system observability
- Application performance monitoring
- Microservices tracing
- Request flow tracking
- Trace analysis and correlation

### Exclusion Examples
❌ **Exclude:** Papers using "distributed tracing" in other contexts:
- **Earth Science:** "Distributed tracing of groundwater contamination"
- **Materials Science:** "Distributed tracing of crack propagation"
- **Biology:** "Distributed tracing of neural pathways"
- **Physics:** "Distributed tracing of particle trajectories"

### Sample Manual Review Process

**Paper Example 1:**
```
Title: "Efficient Distributed Tracing for Microservices Architecture"
Abstract: "...monitoring distributed applications...observability..."
Decision: ✅ INCLUDE (clearly about system tracing)
```

**Paper Example 2:**
```
Title: "Distributed Tracing of Heavy Metal Contamination in Soil"
Abstract: "...environmental monitoring...soil analysis..."
Decision: ❌ EXCLUDE (environmental science, not systems)
```

---

## Data Processing Script Examples

### Author Name Deduplication
```python
# Example of author normalization logic
def normalize_author_name(author):
    """
    Normalize author names to handle variations
    """
    # Remove extra whitespace
    normalized = ' '.join(author.split())
    
    # Handle name order variations
    if ',' in normalized:
        parts = normalized.split(',')
        if len(parts) == 2:
            # "Last, First" -> "First Last"
            normalized = f"{parts[1].strip()} {parts[0].strip()}"
    
    return normalized.title()

# Example data
authors = ["John Smith", "Smith, John", "john smith", "John  Smith"]
normalized = [normalize_author_name(author) for author in authors]
# Result: ["John Smith", "John Smith", "John Smith", "John Smith"]
```

### Institution Standardization
```python
# Example institution mapping
institution_mapping = {
    "MIT": "Massachusetts Institute of Technology",
    "Stanford University": "Stanford University",
    "Stanford CS": "Stanford University",
    "Google Inc.": "Google",
    "Google LLC": "Google",
    "Microsoft Corporation": "Microsoft",
    "Microsoft Research": "Microsoft"
}

def standardize_institution(institution):
    """Standardize institution names"""
    for key, standard_name in institution_mapping.items():
        if key.lower() in institution.lower():
            return standard_name
    return institution
```

---

## How to Reproduce This Study

1. **Clone this repository**
   ```bash
   git clone https://github.com/ylyPikachu/DistributedTracing
   ```

2. **Follow search methodology**
   - Use the search URLs and parameters documented above
   - Apply the same manual filtering criteria
   - Run the data processing scripts
   ```
3. **Generate analysis**
   ```bash
   python Distributed-Tracing-Literature-Analysis.ipynb
   ```
   

For questions about methodology or reproduction, please open an issue or contact liying67@uw.edu.
