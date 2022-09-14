# F-DAL
f - Domain Adversarial Learning

fDAL is a general algorithm that minimizes the discrepancy between the two domains

Trained on MNIST Digits, test on USPS digits dataset.
MNIST->USPS

The following is the optimization problem...

$$\min_{\hat{h}\in \hat{\mathscr{H}}, g\in \mathscr{G}}\max_{\hat{h'}\in \mathscr{H}}  \mathbb{E}_{x\sim p_s}[\mathscr{l}(\hat{h}\circ g, y] +    \mathbb{E} _{x\sim p_s}[\hat{\mathscr{l}}(\hat{h'}\circ g, \hat{h}\circ g)] - \mathbb{E} _{x\sim p_t}[(\phi ^{*}\circ \hat{\mathscr{l}}) (\hat{h'}\circ g, \hat{h} \circ g)]$$

Paper: https://arxiv.org/pdf/2106.11344.pdf
