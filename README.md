# Article-Ranking-with-Location-based-Weight

The full_rank.csv file encompasses a comprehensive ranking system developed to evaluate entities within a network, utilizing various metrics that reflect their importance, impact, and connectivity. This file is a culmination of advanced network analysis techniques, focusing on both traditional and context-aware metrics. Below is a breakdown of the key metrics included in the file:

Key Metrics:
CPR (Context-aware PageRank): This metric extends the traditional PageRank algorithm by incorporating context-aware considerations. It assigns a value to nodes (entities) within a network based on their importance, factoring in the specific context in which they are cited or linked. CPR aims to provide a more nuanced understanding of an entity's significance within a particular domain or topic.
PR (PageRank): The original PageRank value, calculated without context-aware enhancements. It reflects the overall importance of nodes in the network based on their link structure, serving as a baseline for comparison with CPR.
MSC (Multi-Section Citation Count): This metric counts the number of times an entity is cited across multiple sections, aiming to capture its broader impact or relevance across different topics or areas within the network.
TC (Total Citations): The total number of citations an entity receives, providing a straightforward measure of its overall visibility and influence within the network.

Ranking Metrics:
For each of the key metrics (CPR, PR, MSC, and TC), the file also includes corresponding rankings, denoted as follows:
RCPR: The rank of entities based on their CPR values.
RPR: The rank of entities based on their PR values.
RMSC: The rank of entities based on their MSC counts.
RTC: The rank of entities based on their TC counts.


scopus_article.json file is the dataset used for analysis and was obtained using the Scopus API, focusing on Journal of Informetrics Volume 7, Issue 1 to Volume 16, Issue 3. This dataset contains 818 papers and 13,257 references from these papers.


Section_check.csv file provides a granular view of how papers cite each other, broken down by the specific sections in which these citations occur. It's a valuable resource for conducting detailed citation analysis, understanding the context of citations, and examining the flow of information within and across academic documents. Below, we detail the structure and significance of this dataset.

Dataset Columns:
citing_paper_DOI: The Digital Object Identifier (DOI) of the paper that is making the citation. This unique identifier ensures precise reference to the citing paper.
cited_paper_DOI: The DOI of the paper being cited. Like the citing paper's DOI, this unique identifier allows for accurate tracking of the cited document.
Conclusion, Discussion, Introduction, Method, Result: These columns represent the different sections within a paper. Each column contains a count of how many times a cited paper is referenced within that specific section of the citing paper. This breakdown can offer insights into the context and relevance of the cited work.
Total_Count: The total number of sections in which the cited paper appears. This aggregate figure provides a quick overview of the cited paper's overall presence within the citing document.
Appeared_Sections: A list of the types of sections that feature the citation. This column offers a concise summary of where the citations predominantly occur, which can be critical for understanding the context and impact of the cited work.
Importance of Section-Specific Citation Data:
This dataset is especially useful for researchers interested in the nuances of academic influence and information dissemination. By examining citations at the section level, one can understand whether a paper is primarily cited for its methods, results, theoretical contributions, or a combination thereof. Such insights are invaluable for assessing the multifaceted impact of research findings.
