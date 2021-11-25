# QABertEngine

## For create the environement you just need to us the following command

```
pip install -r requirements.txt
```

## For use our code

As for the launching of our code we only have the second one which can be called with the following functions: 

```
dataset = create_the_whole_context_dataset(model_name)
```

With model name a string that represents a model name available in the sentence_transformers lib.

```
knn_model = create_and_train_model(param1, param2, context_list)
```

With param1 and param2 the parameters of hnswlib respectively ef_construction and M.
And context_list need to bes the var dataset define in the previous line of code.

```
result = find_best_context(model_name, knn, question, n, formated_context)
```

With model name a string like in the first line of code (and the same model name is needed).
knn is the knn_model variable defined in the previous line.
question is a string representing the question for which we want to find the most probable context.
n is the number of context we want to get.
And formated_context is the dataset variable defined in the first line.

## code architecture

The archiving of the code is explained in the first part of the report in the 'doc/' folder.
