# What is the Price of a Skill - Data repository.
### When using this data, please cite our work as: Stephany, F., & Teutloff, O. (2024). What is the price of a skill? The value of complementarity. Research Policy, 53(1), 104898. ###

### Variable annotation of skill_dictonary.csv / skill_dictionary.rda

* n_worker: Number of workers possessing each skill.
* n_projects: Number of projects utilising each skill.
* coef: Beta coefficient representing the added value of each skill.
* price: Average monetary value associated with each skill, log(coef).
* premium: A value indicating the premium or extra charge associated with each skill.
* price_level: The average hourly wage of all projects containing a respective skill.
* se: Standard error of the estimated price (coefficient).
* gini: Gini coefficient, typically used to measure inequality, applied here to describe distribution of adjacent skills.
* n_skills: Number of distinct adjacent skills.
* n_clusters: Number of skill clusters of adjacent skills.
* skill: The specific skill.
* ngbr_price: Average price of the three most frequent neighbouring skills.
* ngbr_share: Proportion of the three most frequent neighbouring skills relative to all neighbouring skills.
* ngbr_share_acc: Accumulated share of neighbouring skills.
* ngbr_name: Name of the three most frequent neighbouring skills.
* ngbr_price_res: Residual of the regression “ngbr_price ~ log(price_level)”.
* degree: Simple degree centrality of each skill in the network of skills, indicating the number of direct connections.
* between: Betweenness centrality, which measures the number of times a node appears on the shortest path between other nodes.
* closeness: Closeness centrality, indicating how close a node is to all other nodes in the network.
* eigenvector: Eigenvector centrality, which considers not only the number of connections a node has but also the quality of these connections.
* pagerank: PageRank centrality, derived from the algorithm used by Google to rank web pages.
* cluster: Skill cluster ID of the cluster to which a skill belongs.
* cluster_name: Skill cluster ame of the cluster to which a skill belongs.
* degree_weighted: Weighted degree centrality, taking into account the strength or weight of the connections.
* pagerank_weighted: Weighted PageRank centrality.
* ai_skills: A binary indicator (0 or 1) showing whether a skill is considered an AI-related skill.

### The file edge_list.csv contains the edge list of skills used to create the network of skills. Weights refer to the number of projects that skills have been jointly applied in.
