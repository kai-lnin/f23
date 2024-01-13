Kailin Xia
kailinxi@usc.edu

Dataset: Indicate the dataset you chose to use, any preprocessing steps that were applied, as well as the reasoning behind these choices.

The datasets I chose to use is News Headlines for Sarcasm Detection dataset. For preprocessing, I tokenized the data and added special tokens to fit BERT. I also had to split the data into test, validation, and train sets.

Model Development and Training: Discuss your model implementation choices, the training procedure, the conditions you settled on (e.g., hyperparameters), and discuss why these are a good set for your task.

I chose the pretrained BERT because of its contextual understanding of language, specifically with ‘bert-base-uncased’. After tokenizing and splitting the data, I optimized the model parameters with AdamW to fine-tune pretrained transformers. For batch size, I chose 128 due to the large nature of the dataset.

Model Evaluation/Results: Present the metrics you chose and your model evaluation results. 

I used MCC to indicate prediction performance. My model’s total MCC was 0.876

Discussion: 
How well does your dataset, model architecture, training procedures, and chosen metrics fit the task at hand? 

I feel my model and dataset fit the task at hand sufficiently. However, I know there are ways to improve the model as I gain more familiarity and understanding.

Can your efforts be extended to wider implications, or contribute to social good? Are there any limitations in your methods that should be considered before doing so?

In detecting sarcasm, it can lead to better “Fake News” filtering on search engines such as Google or Bing. Detected sarcasm under the News category could be displayed lower than non sarcastic headlines. This can be a facilitator which pushes factual information to users, and encourages higher media literacy. Some limitations in my methods is certainly a lack of diverse data. The dataset consists of Onion and various other News outlets, but it is not comprehensive enough to cover all media headlines for a search engine. The hyperparameters can also be tweaked to ensure a faster, more accurate prediction in my model.

If you were to continue this project, what would be your next steps?

I would seek for other datasets which covers a wide range of headlines. I would also find ways to preprocess the data, breaking it into segments that could potentially make the model more efficient.
