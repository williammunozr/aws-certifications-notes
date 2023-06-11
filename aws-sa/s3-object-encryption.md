# S3 Object Encryption

| Method                 | Key Management | Encryption Processing |                  Extras                  |
|:-----------------------|:--------------:|:---------------------:|:----------------------------------------:|
| Client-Side Encryption |      YOU       |          YOU          |         S3 never sees plaintext          |
| SSE-C                  |      YOU       |          S3           |                                          |
| SSE-S3                 |       S3       |          S3           |  No Key Control<br/>No Role Separation   |
| SSE-KMS                |    S3 & KMS    |          S3           | Key Rotation Control<br/>Role Separation |