#Importing Data set
World_GDP_Dataset <- read_csv("C:/Users/msrin/Downloads/World GDP Dataset.csv")
World_GDP_Dataset

#descriptive statastics
summary(World_GDP_Dataset[,c('GDP, current prices (Billions of U.S. dollars)','2001')])

#Transformation of variable

df <- World_GDP_Dataset
df$log_2012 <- log10(df$'2012')
df$log_2012

#Plot
plot(df$'2009' ,df$'2013' )
