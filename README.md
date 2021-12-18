# Data-Type-I-Al-Nafi
Data Types and Basic Operations I
  # First Practice
   
  a = 5
  class(5)
  a = 5L
  class(a)
  a = 5 
  class(a)
  x<-c(0.5,0.6)
  class(x)
  x<-c(TRUE,FALSE)
  class(x)
  x<-c(T,F)
  class(x)
  x<-c("a","b","c")
  class(x)
  x<-9:29
  class(x)
  x<-c(1+0i, 2+0i)
  class(x)
  
  
  x<-vector("numeric", length=10)
x


   # Missing Objects
x<-c(1.7,"a")
class(x)
x<-c(TRUE,2)
class(x)
x<-c("a",TRUE)
class(x)



# Explicit Coercion 
    x<- 0:6
   class(x)
   as.numeric(x)
   as.logical(x)   
   as.character(x)
   as.complex(x)
   
   # Nonsensical Coercion
   
  x<-c("a", "b", "c")
  as.numeric(x)
  as.logical(x)
  as.complex(x)  
  
  
  #Matrices 


  m<-matrix(, nrow=2, ncol=3)
  m
  
  m<-matrix(1:6, nrow=2, ncol=3)
  m
  
  dim(m)
  
  attributes(m)
  
  
  m<-1:10
  m  
  dim(m) <-c(2,5)
  m  
  
  #cBinding and rBinding
  
  x<- 1:3
  y<- 10:12
  
  cbind(x,y)
  
  rbind(x,y)
  
  
  #Lists
  
  x<- list(1, "a", TRUE , 1+4i)
  x  
  
  #Factors 
  x<-factor(c("yes", "yes" , "no","yes","no"))
  x  
   
  table(x)
  
  unclass(x)

  
  #Factors Experiment no 2
  x<-factor(c("yes", "yes" , "dont know","yes","no"))
  x  
  
  table(x)
  
  

  
  unclass(x)
  
  
  weekdays<-factor(c("Sunday","Monday","Tuesday","Wednesday","Thrusday","Friday","Saturday"),
                   levels = c("Monday","Tuesday","Wednesday","Thrusday","Friday","Saturday","Sunday"))
  weekdays
  unclass(weekdays)
  
  ################## fACTORS INCLUDE LINEAR MODELING lm()
  #and general linear modeling glm()
  
  #Missing Values
  
  
  x<-c(1,2,NA, 10,3)
  is.na(x)
  is.nan(x)
  
  y<-c(1,2, NaN , NA ,4)
  is.na(y)
  is.nan(y)
  
  
  # Data Frames
  #read.table()
  #read.csv()
  
  x<-data.frame(day=1:4, rain=c(T,T,F,F))
  x
  
  nrow(x)
  ncol(x)  
  
  
  x<- data.frame(day=1:4, rain=c(T,T,F,T))
  x
  nrow(x)
  ncol(x)
  row.names(x)<-c("A","B","C","D")
  x
  
  
  
  
  
                      #NAMES
  x<-1:3
  names(x)  
  
  names(x)<-c("col_A","col_B","col_C")
  x
  
  names(x)
  
  
  
  
  
                      #LISTS
  x<-list(a=1, b=2, c=3)
  x  

  
  x<-list(a=1:5,b="ID", c="names")
  x  
  
  x<-list(a=1:5,b="ID", c=c("first name","last name"))
  x  
  
  x$c
  x$a  
  x$b  

  
  # Name & Matrices  
  m<-matrix(1:4, nrow=2, ncol=2)
  m  
  dimnames(m)<- list(c("a","b"),c("c","d"))  
  m  
  
  
  mk<-matrix(1:4, nrow=2, ncol=2)
  
  dimnames(mk)<- list(c("r1","r2"),c("c1","c2"))
  mk  
  
