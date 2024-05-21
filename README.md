# Medical-Assistant

* The given dataset had two columns for question and answer. The same questions were repeated multiple times with different answers, so first, similar questions were aggregated and combined the answers for them.
* Used the given dataset to train the `BART` model and tokenizer.
* I also tried with `T5` but gave a meager score. Can't use `bert` as it works well on a dataset given context and question as input to find an answer in that context.
* This model gave training and validation loss as:
  
  ![medical_error](https://github.com/garvit088/Medical-Assistant/assets/97309123/760b52c8-a874-4234-8b8f-79fbaa2eb868)

* For training the model, I have used a batch size of 16 for both datasets and epochs, which are set to be 5; more than that would have cost me more computational power and time.
* Used this model to predict on some medical-based questions:
  ![medical_pred](https://github.com/garvit088/Medical-Assistant/assets/97309123/e3390abd-e6eb-4592-a0dd-30c2d51cef30)

