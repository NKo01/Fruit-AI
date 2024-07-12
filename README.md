![image](https://github.com/NKo01/Fruit-AI/assets/175230124/6e6d5efe-6069-42a9-a945-313f959b82ed)

# Fruit Recognition - AI

## Why did I choose this AI ?
Initially, I aimed for a straightforward theme that aligned with the project's objective: to gain a deeper understanding of AI and machine learning. At first, I considered developing an AI that could classify plants. However, after exploring several datasets, I discovered a dataset focused on fruits. This led me to the idea of creating an AI capable of classifying various types of fruits!

## For what purposes could this AI be utilized ?
A significant potential application of this AI could be to sort products, specifically fruits. Indeed, such an AI system could be implemented in various industries, such as agriculture, retail, and food processing, to automate the sorting and categorization of fruits based on their type, size, ripeness, or quality. This would not only improve efficiency and reduce manual labor but also ensure consistent product quality and facilitate inventory management. Additionally, it could aid in monitoring and reducing food waste by identifying fruits that are still consumable but not visually appealing for sale.

Moreover, as initially intended, this AI could serve an educational purpose due to its use of simple and familiar elements like fruits. This makes it an excellent tool for teaching and demonstrating the principles of AI and machine learning in an accessible and engaging way.

## How those the AI work ?

STEP 1 – Kaggle : dataset

STEP 2 – Folder : sorting dataset + labels

STEP 3 – VSC : dragon drop data set

STEP 4 – (code train)

STEP 5 – VSC : cd to nvidia/jetson-inference/
enter docker container (./docker/run.sh)

STEP 6 – VSC : cd to jetson-inference/python/training/classification (cd jetson-inference/python/training/classification/)
run your script (python3 train.py --model-dir=models/cat_dog data/cat_dog)
specify the value of how many epochs and batch sizes you want to run. (--batch-size=NumberOfBatchFiles --workers=NumberOfWorkers --epochs=NumberOfEpochs)

STEP 7 – VSC : I EXPORTING I enter docker container (./docker/run.sh)
Run the onnx export script (python3 onnx_export.py --model-dir=models/cat_dog)

Look in the jetson-inference/python/training/classification/models/cat_dog folder to see if there is a new model called resnet18.onnx there. That is your re-trained model!

![image](https://github.com/NKo01/Fruit-AI/assets/175230124/99047546-65e5-4024-b9c0-fce2cb821d11)
![image](https://github.com/NKo01/Fruit-AI/assets/175230124/f166b014-3f67-4638-a1c4-598bc4858531)

## Thank YOU !

[View a video explanation here](video link)# Fruit-AI
