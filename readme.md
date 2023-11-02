# Deep Learning Project: Charity Funding Predictor
Neural networks and deep learning were utilized to assess the likelihood of funding success for applications.
Formerly provided funding to more than 34,000 organizations through Alphabet Soup.
## Processing Data
Since the dataset eliminated any unnecessary data, the EIN and NAME were eliminated from the model. The following columns were thought of as the model's features. Despite this, NAME was added once more in the second test. Because of the significant fluctuation, CLASSIFICATION and APPLICATION_TYPE were swapped out for "Other." The data was divided into sets for testing and training. The "IS_SUCCESSFUL" target variable for the model is validated by the value, where 1 denotes "yes" and "0," "no." After analysis of the application data, CLASSIFICATION's value was used for binning. Each unique value binned "rare" category variables together into a new value called "Other" by using many data points as a cutoff point. Later verified that the binning process had been successful. The encoding of categorical variables used by `pd.get_dummies()`.
## Compiling, Training, and Evaluation the Model
Three layers of neural networks were applied to each model. The quantity of hidden nodes was determined by the characteristics.
477 parameters were produced by a training model with three layers. At 72%, the first attempt was nearly successful, but it fell short of the intended 75%.
## Optimization
After adding "NAME" back into the dataset in my second attempt, I was able to achieve 78%, which was 3% above my goal.
Since deep learning is machine-based and teaches a lot of concepts, it should have several layers, allowing the computer to sort through layers of inputs and learn how to categorize and anticipate data.