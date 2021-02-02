# Artificial_Intelligence_for_Knowledge_Discovery

In this project, the objective is to build a simple end to end pipeline in order to extract
knowledge from a set of documents, represent this knowledge using rdf, query the created rdf
graph and eventually use reasoning to enrich the extracted knowledge.
Before starting the implementation of your pipeline. You should collect 30 news articles about
different topics from different websites.
In order to build the whole pipeline, you will need different subparts :
1. Collect 30 news articles and save them in a forlder, you can name them using this
pattern : ”id_title_class”.txt
2. A program that trains a model to classify news document in order to predict the main
topic of it
3. A program that takes as input a document (or a list of documents contained in a
directory) and output in a csv file the document class (predicted by the model), and
eventually the date creation, the title, the authors or any other information that you can
extract
4. A program that takes as input the document, the document ID and the label predicted by
the learned model. This program should output an RDF file.
5. Optional :
a. You can do some topic modelling to extract more knowledge about the
documents
b. You can also perform Named Entity Recognition using some pretrained models
in NLTK or Spacy
6. A program that contains generic sparql queries that will be executed on the rdf file once
loaded in a Jena model.
7. A program that will take an ontology modeling some class hierarchies (example : basket
is subclassof sport) about the labels you have, the rdf file and will perform reasoning in
order to enrich the extracted knowledge.
8. Optional : You can run some queries over the dbpedia (or any other Linked Open
Dataset) to get more knowledge about the topics you extract from document.
