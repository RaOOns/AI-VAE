# AI-VAE: Auxiliary Information variational autoencoder

- I developed a book lending recommendation system called Auxiliary Information variational autoencoder(AI-VAE).

- AI-VAE used Multi-VAE as a base model and improved its performance by adding user and item(book) information.

- As evaluation metrics, Normalize Discounted Cumulative Gain(NDCG) considering the recommendation order and HIT rate not considering the recommendation order were used, and the performance was compared with Multi-VAE and RecVAE.

<p align="center"><img src="https://user-images.githubusercontent.com/79679194/229520741-b9f50e02-965b-448a-96c8-04b333ce883a.png" height="250px" width="400px"></p>

### The dataset information is as follows:
- **Lending matrix:** This matrix indicates whether the user has borrowed the book (1 if borrowed, 0 if not).

- **User information:** Gender, Year of born.

- **Book information:** Publish year, Korean book classification criteria, book classification title, International Standard Book Number (ISBN13), title, author, publisher, volume, single ISBN13 sign.

- **Derived variables:** Country of publication, Cumulative number of book lending by book.



### Reference
- AI-VAE: https://m.riss.kr/link?id=T16622597
- Multi-VAE: https://doi.org/10.48550/arXiv.1802.05814
- RecVAE: https://doi.org/10.1145/3336191.3371831
