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

####Finding max value in row
row_index = y.argmax(axis=0)

#####Converting to cumulative days

temp <-  data.frame(rul)
temp$failure <- as.character(temp$failure)
str(temp)

seq_of_fail <- function(x){
  j <- 0
  for (i in 1:nrow(x)){
    if(x[,7][i]=="none"){
      j<- j+1 
      x[,8][i] <- j
    }
    else{
      x[,8][i] <- 0
      j <- 0
    }
  }
  return(x)
}


z <- seq_of_fail(temp)

#####################################################
##Creating sequence of ids
custo_freq <- data.frame(table(new_train$people_id))
bind <- sapply(custo_freq[,2],function(x) seq(1,x))
dd <- data.frame(unlist(bind))
####################################################
mode of dataframe rows
ensemble_model[['PREDICTED_Class']] <- apply(ensemble_model,1,function(x)  {tab <- table(x); names(tab)[which.max(tab)]})
