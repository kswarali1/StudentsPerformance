# StudentsPerformance
ggplot(data=avg_math, aes(x=gender, y=avg_math), main="Average Math Scores") + geom_bar(stat="identity")
ggplot(data=avg_reading, aes(x=gender, y=avg_reading), main="Average Reading Scores") + geom_bar(stat="identity")
ggplot(data=avg_writing, aes(x=gender, y=avg_writing), main="Average Writing Scores") + geom_bar(stat="identity")
