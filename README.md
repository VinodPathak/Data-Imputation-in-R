#Data Cleaning

####Data-Imputation-in-R
Impute with Mode
s.numeric(names(sort(-table(column_name)))[1])

#####Delete columns using Pandas
df[df.columns-["column1","column2"]]


#####String to numeric conversion in Pandas
from sklearn import preprocessing
label_encoder = preprocessing.LabelEncoder()
df["religion"] = label_encoder.fit_transform(df["religion"])
