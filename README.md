# credit-risk-classification
Overview of the Analysis:

This analysis delved into the effectiveness of two machine learning models using financial data to predict loan risk. Our primary objective was to ascertain whether loans could be classified as high-risk or healthy (low-risk), a crucial aspect in financial sectors for robust risk management and decision-making processes. After thorough examination of various predictive variables, two models were developed to comprehend the distribution of risk across loans. The dataset initially comprised 75,036 healthy loans and 2,500 high-risk loans.

Results:

•Model 1 (Without Resampling):
The logistic regression model exhibited remarkable accuracy. It achieved flawless precision and recall for healthy loans (class 0), denoting exceptional performance in correctly classifying these cases without any false positives or negatives. For high-risk loans (class 1), the model's precision was 0.85, indicating an 85% accuracy when predicting high-risk loans. Its recall was 0.91, capturing 91% of all actual high-risk loans.

•However, Model 1 underclassified high-risk loans by 15%, raising concerns about its practical applicability. Misclassifying a high-risk loan as healthy could result in substantial financial consequences if the loan defaults. Despite its robustness, the model's tendency to underclassify high-risk loans necessitates careful consideration. Adjusting the prediction threshold or incorporating the model's predictions into a broader decision-making framework that factors in potential monetary risks may be imperative.

•Model 2 (With Oversampling):
Following the implementation of oversampling techniques, Model 2 demonstrated a much-improved balance. The recall for high-risk loans (class 1) surged to an impressive 99%, signifying a considerable enhancement. Although there was a marginal decrease in precision (by 1%), this tradeoff was deemed acceptable. The model became more discerning, classifying healthy loans as high risk with rare occurrence while significantly reducing instances of high-risk loans being misclassified as healthy.

•Interestingly, predictions for class 0 remained stable even after oversampling, ensuring the model's continued accuracy in identifying healthy loans. This balanced performance underscored Model 2's reliability and precision in classifying loans accurately, making it a prudent choice for risk mitigation.

Recommendation:

Considering the enhanced balance, improved risk mitigation, and reduced false negatives, Model 2 stands out as the superior choice for practical application. To further validate the model's accuracy, I would recommend conducting comparative studies between the model's predictions and the company's manual evaluations. This validation process will ensure the model's effectiveness and provide valuable insights into refining the risk assessment process.