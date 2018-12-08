## StudentsPerformance

#Bar Graph for Average Math Scores based on Gender
ggplot(data=avg_math, aes(x=gender, y=avg_math), main="Average Math Scores") + geom_bar(stat="identity")+ ggtitle("Average Math Scores")

#Bar Graph for Average Reading Scores based on Gender
ggplot(data=avg_reading, aes(x=gender, y=avg_reading), main="Average Reading Scores") + geom_bar(stat="identity")+ ggtitle("Average Reading Scores")

#Bar Graph for Average Writing Scores based on Gender
ggplot(data=avg_writing, aes(x=gender, y=avg_writing), main="Average Writing Scores") + geom_bar(stat="identity")+ ggtitle("Average Writing Scores")

#Compare Math and Reading Scores based on Gender
math_reading <- merge(avg_math, avg_reading, by="gender")

#Compare Writing and Reading Scores based on Gender
reading_writing <- merge(avg_writing, avg_reading, by="gender")

#Compare Math and Writing Scores based on Gender
math_writing <- merge(avg_math, avg_writing, by="gender")
