# multi-database-financial-merge
This project merges CRSP/Compustat (CCM), SDC M&amp;A, IBES, MSCI ESG, and BoardEx datasets for 2019–2024 using high-quality firm identifiers and link scores. It integrates financial, market, ESG, and governance data to build a unified research panel for empirical asset pricing and corporate finance studies.

This project performs a comprehensive multi-database merge across CRSP/Compustat (CCM Spine), SDC M&A, IBES Price Target, MSCI ESG, and BoardEx Analytics data for the period January 1, 2019 – December 31, 2024.

The merge links key financial, accounting, analyst, ESG, and governance datasets using consistent firm identifiers and link scores.

CRSP/Compustat (CCM Spine): Core financial and market variables (as used in Week 3).

SDC M&A: Complete deal-level variables.

IBES Summary History – Price Target: Analyst expectations; limited to best CRSP/IBES links (score = 1).

MSCI ESG: Core identification fields plus key ESG metrics (IVA ratings, pillar scores, weighted averages, and environmental/social/governance weights).

BoardEx – Organization Summary: Governance and board characteristics, limited to best CRSP/BoardEx links (score = 1).

The project includes careful identifier standardization (GVKEY, PERMNO, CUSIP, TICKER, company name) and ensures date alignment across data sources. Records with missing or low-quality links are excluded. The final dataset is designed to support empirical research in ESG performance, M&A activity, and market-based valuation.

The code is implemented in SAS, with validation checks for matched, unmatched, and overlapping records.
