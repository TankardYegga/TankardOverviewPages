- A. About the method section:
- (1) There are inconsistencies in the description:
	- 1) in "3.3. Quantitative Analysis of Feature Parameters", roundness is denoted as S, but in "The closer the resulting value of circularity", S is referred to as circularity;
	- 2) "n represents the number of attributes of the data sample" contradicts "B = {b1, b2, ..., bn}", where n tends to be understood as the number of samples in the later description.
- (2) There are places where the description is not clear:
	- 1) What is the meaning of the summation in Equation 6? Is the upper limit of the summation of Equation 6 the S in Equation 4?
	- 2) How are the four weights w1, w2, w3, and w4 calculated?
	- 3) Are the two analysis techniques for improved Bayesian proposed by you? Why not point out the innovation points in the contribution?
- (3) Your method here is not a deep learning model, but a traditional machine learning model. Why do you need to use PyTorch to implement it?
-
-
- B. About the text
- (1) Some sentences are written in a style of Chinese language
	- For example, "high accuracy ultrasound image classification" in the abstract is recommended to be changed to "high accuracy in the classification of ultrasound images"
- (2) There is a syntax error
	- "To obtain more accurate and efficient image feature classification results." cannot stand alone as a sentence;
	- "As shown in Figure2." also cannot stand alone as a sentence.
- (3) The meaning of some sentences is repeated or even redundant, which is not concise enough
	- In "improve the classification accuracy and enhance the accuracy of diagnosis",  the diagnosis accuracy and classification accuracy here seem to be the same concept;
	- The sentence "this study applied the improved Navie Bayesian algorithm to feature classification and applied it to quantitative feature classification of breast ultrasound imaging" contains repetition and can be changed to "this study applied the improved Navie Bayesian algorithm to quantitative feature classification of breast ultrasound imaging".
- (4) Several sentences are too long
	- Use "and" in many places to connect three or four verb phrases, such as "it can effectively avoid the influence of external factors, improve the sensitivity of breast tumors and other types of lesions, and reduce the probability of misdiagnosis and missed diagnoses".
- (5) The content of the sentence is mixed, making it difficult to understand
	- Contribution 3) mix the evaluation index and the experimental purpose together, preferably separately;
	- In the sentence "The results show that the contour of the lesion recognition results obtained by the proposed algorithm is the most complete, and the other regions can maximize the retention of the texture features of the original image, the accuracy value is 85.3, the sensitivity value is 85.6.", it is better to separate qualitative and quantitative results;
	- In the literature review, there are too many contents of each literature, and it is difficult for readers to find the key points;
-