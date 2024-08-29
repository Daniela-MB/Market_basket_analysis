## Introduction

Market Basket Analysis, also known as association-rule mining, examines transactional data to uncover customer purchasing patterns. This analysis helps retailers gain a competitive advantage by understanding typical purchase behaviors, which can enhance store layouts, website designs, and marketing strategies, such as promoting bundled offers (Chen et al., 2005, p.339)..
This project will focus on two algorithms: Apriori and Frequent Pattern Growth (FP-Growth).

## Objective
To leverage the insights gained from these algorithms to boost sales, enhance customer experience, and optimize operational efficiencies in the online electronic store.

## Dataset
The <a href="https://www.kaggle.com/datasets/farjanakabirsamanta/analytics-case-studyecommerce" target="_blank">dataset</a> are from the Kaggle repository and contains e-commerce data from an online electronic store. 

## Project execution

- The CRISP-DM methodology was used for structured and effective project execution.

- EDA and preprocessing were performed to understand data distribution and handle missing values.

- Apriori and Frequent Pattern Growth (FP-Growth) algorithms were used for mining frequent itemsets by setting a minimum support threshold. In this project, identical parameter values were used for both algorithms to ensure a reliable comparison.
  
- The speed test was conducted on these algorithms to provide insights into their practical performance, which is essential for optimizing data processing tasks and ensuring efficient analysis.

## Results

- *Apriori and FP-Growth Algorithms* 
  - These algoritms results were identical, demonstrating that they can consistently identify antecedents and consequents when parameters are the same. However, while the output is similar due to the deterministic nature of both algorithms, their differences lie in efficiency and scalability, which will be explored in the subsequent section on speed tests.
 
- *Speed test: Apriori and FP-Growth*
  - The FP-Growth algorithm (1.78 seconds) is 1.75 times faster than Apriori (3.12 seconds). This faster performance is due to FP-Growth’s use of the FP-tree structure, which reduces database scans and complexity. In contrast, Apriori’s candidate generation and multiple scans make it less scalable and slower, as highlighted by previous studies.
 
## Conclusion

Both Apriori and FP-Growth algorithms produce identical results when using the same parameters, demonstrating their ability to consistently identify antecedents and consequents. However, their efficiency and scalability differ significantly. The FP-Growth algorithm is notably faster, taking 1.78 seconds compared to Apriori’s 3.12 seconds, due to its more efficient FP-tree structure that reduces database scans and complexity. In contrast, Apriori’s reliance on candidate generation and multiple scans leads to slower performance and scalability issues. Thus, while both algorithms are effective in identifying itemsets, FP-Growth is preferable for handling larger datasets and achieving faster processing times.


## References:

Chen, Y.-L., Tang, K., Shen, R.-J. and Hu, Y.-H. (2005). Market basket analysis in a multiple store environment. Decision Support Systems, 40(2), pp.339–354. doi:https://doi.org/10.1016/j.dss.2004.04.009.

Han, J., Pei, J. and Yin, Y. (2000). Mining frequent patterns without candidate generation. ACM SIGMOD Record, 29(2), pp.1–12. doi:https://doi.org/10.1145/335191.335372.

Heaton, J. (2016). Comparing dataset characteristics that favor the Apriori, Eclat or FP-Growth frequent itemset mining algorithms. [online] IEEE Xplore. doi:https://doi.org/10.1109/SECON.2016.7506659.

Hossain, M., Sattar, A.H.M.S. and Paul, M.K. (2019). Market Basket Analysis Using Apriori and FP Growth Algorithm. [online] IEEE Xplore. doi:https://doi.org/10.1109/ICCIT48885.2019.9038197.

Numpy (2009). NumPy. [online] Numpy.org. Available at: https://numpy.org/. [Accessed 16 May 2024].

OpenAI. (2024). ChatGPT (GPT-3.5 version) [Large language model]. https://chat.openai.com/chat (https://chat.openai.com/chat. [Accessed 20 May 2024])

pandas.pydata.org. (n.d.). User Guide — pandas 1.0.4 documentation. [online] Available at: https://pandas.pydata.org/docs/user_guide/index.html#user-guide. [Accessed 16 May 2024].

Shankar (2024). Apriori vs. FP-Growth: Comparative Study of Data Mining Algorithms - Algorithmic Mind. [online] Algorithmic Mind. Available at: https://algorithmicmind.org/difference-between-apriori-and-fp-growth/ [Accessed 22 May 2024].
