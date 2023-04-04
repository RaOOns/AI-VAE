# AI-VAE: Auxiliary Information variational autoencoder

- I developed a book lending recommendation system called Auxiliary Information variational autoencoder(AI-VAE, https://m.riss.kr/link?id=T16622597).

- AI-VAE applied the VAE of a neural network based recommendation system.

- The base model was Multi-VAE(https://doi.org/10.48550/arXiv.1802.05814) and its performance was improved by adding user and item(book) information.

- As evaluation metrics, Normalize Discounted Cumulative Gain(NDCG) considering the recommendation order and HIT rate not considering the recommendation order were used, and the performance was compared with Multi-VAE and Rec-VAE(https://doi.org/10.1145/3336191.3371831).

<p align="center"><img src="https://user-images.githubusercontent.com/79679194/229520741-b9f50e02-965b-448a-96c8-04b333ce883a.png" height="250px" width="400px"></p>

<br/>

### The dataset information is as follows:
- **Lending matrix:** This matrix indicates whether the user has borrowed the book (1 if borrowed, 0 if not).

- **User information:** Gender, Year of born.

- **Book information:** Publish year, Korean book classification criteria, book classification title, International Standard Book Number (ISBN13), title, author, publisher, volume, single ISBN13 sign.

- **Derived variables:** Country of publication, Cumulative number of book lending by book.

<br/>
  
### Performance and Opinion
-  In the case of HIT rate without considering the recommendation order, AI-VAE showed the best performance.

- In the case of NDCG considering the recommendation order, AI-VAE showed the second performance.

- AI-VAE is affected by auxiliary information from the user and the item. Therefore, if the auxiliary information is supplemented, the performance is expected to be further improved.


![AI-VAE 성능 결과 1](https://user-images.githubusercontent.com/79679194/229666500-558159b0-52ed-4202-a7eb-b52c03ddb7f2.png) |![AI-VAE 성능 결과 2](https://user-images.githubusercontent.com/79679194/229666538-2097bef0-3db1-4d33-8025-42e67b0d239d.png)
--- | --- | 

<br/>

### Reference
- AI-VAE: https://m.riss.kr/link?id=T16622597
- Multi-VAE: https://doi.org/10.48550/arXiv.1802.05814
- RecVAE: https://doi.org/10.1145/3336191.3371831
