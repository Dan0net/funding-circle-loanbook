# Funding Circle Loanbook Analysis

[This ipython notebook](https://github.com/Dan0net/funding-circle-loanbook/blob/master/LoanBook%20Analysis.ipynb) predicts the outcome of loans on Funding Circle's live Loan Requests page.

### How to use
Run the code through to the end to get live results for the loans listed on https://www.fundingcircle.com/lend/loan-requests/.

## How it works
- The model is an AdaBoost ensemble regressor, that learns from [Funding Circle'sloan book](https://www.fundingcircle.com/loanbook) to make estimations based on the information available on the Loan Requests page.

- The model estimates 5 different types of outcome `success`, `defaulted`, `repaid`, `late` and `repaying`.

- A loan is 'successful' if it is likely to be fully repaid, or has passed 50%  of it's repayment term without defaulting or being late.

- The learnt model is around 83% accuracy for `success` predictions, 87% for `defaulted`, 80% for `repaid`, 95% for `late` and 97% for `repaying`.

- The 5 outcome types are all inter-dependent in different ways, so they don't add up to 100%. They only give indications about the likely performance of the loan, and do not indicate a direct outcome.

### Discussion & Feedback
A [forum thread is here](https://forum.fundingcircle.com/discussion/13480/estimate-loan-outcomes-and-loan-book-analysis/p1?new=1).

Please let me know if you find it helpful and feel free to suggest improvements or create pull requests! The model is fairly basic so there's load of room for improvement, I'd really appreciate any feedback.

I hope you find it useful in your bidding - but I don't take any responsibility for your bad debt!

##### Author
Daniel Martinho-Corbishley
