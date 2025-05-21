# Stock-Pair-Similarity-Analysis-Inspired-by-Gene-Co-Expression-Networks
 This project identifies and analyzes the most closely correlated stock pairs in the NASDAQ-100, using daily return data over the past 3 years. The goal is to discover which stocks move together most tightly — both in direction and in magnitude — similar to how gene co-expression networks reveal biologically linked genes.

Key Features

    ✅ Downloads daily price data using yfinance

    ✅ Calculates pairwise Pearson correlation of returns

    ✅ Ranks stock pairs by rolling standard deviation of return differences (low deviation = tighter tracking)

    ✅ Visualizes:

        Correlation barplots

        Deviation vs. correlation dual-axis plots

        Clustermap of top stock correlations (bio-inspired)

        Gene-network-style co-movement graph (modular, colored by cluster)

Bio-Inspired Twist
This notebook borrows from techniques in computational biology:

    Gene co-expression → Stock co-movement

    Module detection → Stock clusters

    Phylogenetic tree → Stock dendrogram

Usage

    Change the START_DATE, END_DATE, NUM_STOCKS, or correlation threshold to explore different periods or subsets.

    Try adjusting the network graph to test different co-movement strengths.

Why 49 and not 50 stocks?
We removed one of Alphabet Inc.'s duplicate share classes (GOOGL vs. GOOG) to avoid inflating correlations between two stocks that reflect the same underlying company.
