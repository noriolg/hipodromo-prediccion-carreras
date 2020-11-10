# Hipódromo

The aim of this side project is to build a model that can help predict the winning horse for races in Hipódromo de la Zarzuela (Madrid). 
This is a long term project and it is not sure that the results will be satisfactory.

For now, the data gathering and scraping process is still undergoing. I currently have no clue on how to proceed one I have enough data so I will be doing some more research on the topic. 

Some doubts I have are:
* When bilding the model, horses in your race matter a lot so somehow it would be necessary to individually consider each race.
* How to account fot the other horses in the same race when training the model?
* Any other factors that influence?

Planned next steps:
* Find more information about the trainer/owner of the horse and substitute that info for their name in the tables.
* Map weather to each of the races

**Update!**
I found an example that gives some hints on how to solve the problems stated earlier. 
It seems that by treating all horses from the same race as one observation and running a neural network you are accounting for the fact
that only other horses from the same race influence your current performance. See [here](https://towardsdatascience.com/use-machine-learning-to-predict-horse-racing-4f1111fb6ced) 
for more explanation.

I will be trying this out after I add some new features and trying to look for more information about the trainers and jockeys. Also, I am thinking that I need
to figure out a way to prevent overfitting...
