# CaseStudy2DDS
Executive Summary:

Many trends and Analysis can be discovered when experimenting with a collection of data set provided.  A really great example of this is about to be
displayed in this project I am about to unfold.  A significant amount of data on employees of a company was given and that data was used to conduct the findings that
I will be explaining in this case study presentation.  

Intro:

After conducting some much needed research and using several coding models to analyze the data given, it 
was found that there were a few factors within a company that could lead to attrition in a place of business.
The company that I will be experimenting with today is your company, which is Frito Lay.  

Coding used:

summary(CaseStudy2_data)

# Read in CaseStudy2 data set
CaseStudy2_data <- read.csv(file.choose(),header = TRUE)

ggplot(CaseStudy2_data,aes(x = WorkLifeBalance, y = YearsAtCompany,color = Age)) + geom_point()

# Scatter plot with LR model overlay
CaseStudy2_data %>% ggplot(aes(x=Age, y=YearsAtCompany)) + geom_point() + ggtitle("LR Model: Age vs YearsAtCompany") + geom_smooth(method = "lm")

# Scatter plot to inspect general trend
CaseStudy2_data%>%ggplot(aes(x = TotalWorkingYears, y = Age)) + geom_point() + ggtitle("TotalWorkingYears vs Age")


[Tonya.Belk_Case Study 2.pptx](https://github.com/tonyabelk/Case-Study-2/files/7655750/Tonya.Belk_Case.Study.2.pptx)

https://youtu.be/OJzWVOFxnw0

