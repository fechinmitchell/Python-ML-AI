# Python-ML-AI
Machine Learning and AI in Python

I will run my first Machine Learning Algorithm, I will use a decision tree as my classifier and my target will be determining a label, Man or Woman from a set of three attributes Height, Weight, Shoe Size.

First Step: Make sure Python is available for use on your operating systems, Windows user will have to donwload and install it, Mac and Linux user will have it pre-installed.

Second Step: Use text editor like sublime text or the one I like to use is Jupyter Notebook which is run from the terminal when you type "jupyter notebook".

Third Step: Run the code below line by line to see how the decision tree works, use different values in the in the prediction line to verify the code is running correctly.




from sklearn import tree

clf = tree.DecisionTreeClassifier()

#Height, Weight, Shoe Size
X = [[181, 80, 44], [177, 70, 43], [160, 60, 38], [154, 54, 37], [166, 65, 40],
     [190, 90, 47], [175, 64, 39],
     [177, 70, 40], [159, 55, 37], [171, 75, 42], [181, 85, 43]]

Y = ['male', 'male', 'female', 'female', 'male', 'male', 'female', 'female',
     'female', 'male', 'male']

clf = clf.fit(X, Y)

prediction = clf.predict([[180, 70, 43]])
      
print(prediction)
