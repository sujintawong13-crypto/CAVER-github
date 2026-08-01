## Dataset Field Descriptions

- `Source`: Source from which the citation pair was collected (e.g., `PubPeer`, `Smith & Cumberledge, 2020`).

- `Citing Article DOI`: Digital Object Identifier (DOI) of the article containing the citation statement.

- `Citing Article Title`: Full title of the article that cites another publication.

- `Domain`: Academic discipline of the citing article (e.g., `Physics`, `Biology`, `Medicine`, `Computer Science`).

- `Statement with Citation`: Citation-containing statement extracted from the citing article. The original citation marker is replaced with a placeholder (e.g., `[citation]`, `[citation 49]`).

- `Reference Article DOI`: DOI of the cited (reference) article.

- `Reference Article Title`: Full title of the cited article.

- `Reference Article Abstract`: Abstract of the cited article, used as supporting evidence for citation verification.

- `Label`: Ground-truth citation verification label.
  - `Fully Substantiated`: The cited statement is genuinely supported by the referenced article, either verbatim, semantically equivalent, or partially aligned with the reported findings.
  - `Unsubstantiated`: The cited statement is not supported by the referenced article. This category includes misleading interpretations of the source as well as citations to articles containing no relevant supporting evidence.

- `PDF`: URL to the full-text PDF of the cited article (or another accessible copy) used during the verification process.

- `Explanation`: A natural-language rationale explaining the annotation decision. It summarizes the relationship between the citation statement and the cited article, highlighting whether and why the evidence supports the claim.

- `Evidence`: The evidence passage extracted from the cited article that justifies the annotation. This is typically a verbatim excerpt from the article's abstract, results, discussion, or other relevant sections used for citation verification.
