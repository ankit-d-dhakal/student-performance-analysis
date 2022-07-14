# student-performance-analysis

The dataset used for this analysis is attached here:

[student.csv](https://github.com/ankit-d-dhakal/student-performance-analysis/files/9092035/student.csv)

# 1\. Data Understanding

The provided data is of students' achievement from the two different
schools named "Gabriel Pereira", represented by GP, and "Moushinho da
Silveira", represented by MS in the dataset. The attributes of data
include student grades of mathematics, location of the students, social
activities in which students are involved, and a few of the
school-related features. There are total of 33 attributes. The following
is the tabular representation of details provided in the data set.


# 2\. Further Anaylsis

All the variable type of different columns were identified and converted into numerical values. The types were:

- Categorical
- Discrete
- Ordinal

The categorical data was transformed into 0 and 1 where ordinal values were transformed into numberical values based on total number of unique attributes.

# 3\. Initial Data Analysis

## 3.1 Correlation between the absences, failures, G1, G2 and G3 and presenting them in heatmap

There is inbuilt function in pandas known as **dataframe.corr()** which
will find the pairwise correlation of all columns in dataframe. Any na
values are excluded. It also ignores any non-numeric data type columns
in the dataframe. (GeeksforGeeks, 2020)

![1](https://user-images.githubusercontent.com/29594566/178654350-0336f253-e95e-4342-a96a-3f944d161c14.png)

![image](https://user-images.githubusercontent.com/29594566/178656285-72e4f4bc-1ddd-49b1-9b3d-d07a22f49d68.png)

Above heatmap is based on the correlation between five different
variables which are absences, failures, G1, G2 and G3. If the colour is
dark then the correlation between the variables is strong, if the colour
is light then the correlation between variables is weak. So, from the
figure we can see that G3 and G2 has strong correlation because the
colour representing it is dark whereas correlation between absences and
G2 is weak because the colour representing it is in light comparing to
other.

# 4\. Data Exploration and Visualization

## 4.1 Histogram plot and boxplots for age, absences and G3

### 4.1.1 Histogram plot for age


![3](https://user-images.githubusercontent.com/29594566/178654699-ca045c92-f779-43ea-9e7a-f917f295024e.png)

From above histogram plot we can see that the majority of students age
is in between 16 and 18 and minority of age is from 20 to 22.

###  4.1.2 Histogram plot for absences


![4](https://user-images.githubusercontent.com/29594566/178654770-f7f483e6-cd4d-44e4-a15a-4124ea092925.png)

From above histogram plot we can see that the majority of students are
absent for around 5 days and minority of students are absent for 75 to
80 days.

###  4.1.3 Histogram plot for G3

![5](https://user-images.githubusercontent.com/29594566/178654833-b4166b1f-d9dc-4735-acd9-f0242101c9e6.png)

From above histogram plot we can see that the majority of students have
secured final grades between 10 and 15 whereas there are few numbers of
students who have secured grades between 20 and 25.

### 4.1.4 Boxplot for age


![6](https://user-images.githubusercontent.com/29594566/178654897-546701c4-0cf0-4a66-b5df-0e4ea9684e00.png)

The above boxplot shows us that the minimum age of student in the school
is 15 and the first quartile start from age of 16 and median is 17.
Third quartile lies in age of 18 and maximum age is 22.

### 4.1.5 Boxplot for absences

![7](https://user-images.githubusercontent.com/29594566/178655063-8cd35f26-8799-47a1-ab86-c5169dcf0265.png)

From above boxplot we can see that minimum number of absent days of
student is 0 whereas median value, first quartile and third quartile lie
between 0 and 10 and maximum value is above 70.

### 4.1.6 Boxplot for G3

![image](https://user-images.githubusercontent.com/29594566/178655179-1325f5a7-1af0-4bb6-91c7-ad387300b475.png)

From above boxplot we can see that minimum number of grades secured by
student is 0 whereas median value, first quartile and third quartile lie
between 7.5 and 15 and maximum grade secured is 20.

## 4.2 Graduation rates by school

![image](https://user-images.githubusercontent.com/29594566/178655199-9f348ee6-4b0d-4a68-abda-79b46e0289cf.png)

The above bar graph provides us the information about the number of
students who has secured passing grades in both GP and MS school. Here,
the students from GP has secured more passing grades compared to MS.

## 4.3 Failures by weekly study time

Bar graph of total number of students who failed the final term grouped according to weekly studytime

![image](https://user-images.githubusercontent.com/29594566/178655226-ad04d169-6ac7-4943-a181-0d3a3b91e8cd.png)

According to above bar graph we can see that the maximum number of
students who have the studytime from 2 to 5 hours per week are failing
their subjects. Whereas the students who have studytime of more than 10
hours are failing less.

# 5\. Further Analysis

## 5.1 Pass and failed rate in both GP and MS School

![image](https://user-images.githubusercontent.com/29594566/178656074-eeb75d4c-83e1-4e3b-9651-9b3674026beb.png)

![image](https://user-images.githubusercontent.com/29594566/178656116-412d9803-6f7b-45e5-b6e5-6a4cd213e4bf.png)

From above findings we can see that pass rate of GP school is high
compared to MS school pass rate whereas coming towards failed we can see
that MS school has higher number of failing rate compared to GP school.
So, from above findings we can conclude that the overall best student
are from school GP.

## 5.2 Grade of Students as per gender


![image](https://user-images.githubusercontent.com/29594566/178655375-300251a0-fcd5-412d-b16d-30b4d50447f3.png)

From above bar graph we can see that in both schools the number of
passed students per male and female is high but if counted in numbers we
can see that female passed rate is slightly more comparing to the males.
And male failed rate is nearly half in numbers compared to the females
failed rate.

So, we can say that the male students are slightly better in studying
after comparing passed and failed rate of females.

## 5.3 How student’s family background is affecting his/her final grade?

### 5.3.1 Grade of students as per father’s job

![image](https://user-images.githubusercontent.com/29594566/178655422-bd3b9db3-cb4f-47c8-916a-c9a7a2c0810f.png)

As we can see that the number of passed and failed student is high whose
father’s job falls in other category, but the number of passed student
is very less whose father does not have any job and father whose job is
in health sector. But looking further the number of failed students is
less whose father job is in health sector comparing to all job
categories.

### 5.3.2 Grade of students as per mother’s job

![image](https://user-images.githubusercontent.com/29594566/178655446-58373955-12e6-4c4b-9bd7-736d2d103dbf.png)

From above countplot we can see that the students whose mother’s
occupation falls under other categories have higher number of passed and
failed records and the students whose mother’s occupation falls under
health categories have lower number of passed and failed records. The
student whose mother’ occupation is in services have slightly less
number of passed and failed record compared to other categories.

In conclusion, both the father and mother whose occupation is in other
categories have higher number of passed and failed record of students.

## 5.4 How Parent’s education background affecting students pass rate

![image](https://user-images.githubusercontent.com/29594566/178655492-3628b78e-332c-4179-992a-ca3d3c7adf4a.png)


![image](https://user-images.githubusercontent.com/29594566/178655505-85d12b79-fc00-4dc2-bfa6-df51a3ad145b.png)

From above two barplots we can see that the number of students whose
father and mother education falls under none category have higher number
of passing rate but in case of higher education qualification of parents
the number of passed student is equal with none. Also, in case of father
who have only primary education qualification the number of failed
student is high comparing to other categories. Looking into mother’s
education qualification the record of failed students is high whose
mother education qualification is higher education.

## 5.5 How parent’s relationship status is affecting their children’s passing rate

![image](https://user-images.githubusercontent.com/29594566/178655579-628baeee-cd09-49d6-a007-286c50fad37d.png)

We can see that the parents whose relation status is considered to be
very good has higher number of passed and failed record of students.
Whereas the pass and fail record of students whose parents’ relation
status is excellent falls right behind the parents having very good
status. On the other hand, parents whose relation status is very bad has
low number of pass and fail record.

In conclusion we can say that the parent’s relation does have direct
effect in student final grade.

## 5.6 How student’s travel time affecting their final grade?

![image](https://user-images.githubusercontent.com/29594566/178655664-1e58a3d4-6cff-4f08-b306-95fe0526a2b6.png)

From above plot we can clearly see that travel time has direct affect on
the students grade because the students whose travel time is more than 1
hour has less number passing record whereas the students whose trave
time is less than 15 mins has the highest number of passing record.
Also, the students whose travel time is from 30 mins to 1 hour has low
number of passing record.

So, we can say that the students travel time between school and their
home does have direct affect

on their ability of passing the exams.

## 5.7 Does hanging out with friends affect the overall grades of the students?

![image](https://user-images.githubusercontent.com/29594566/178655708-e4ad0a5b-e05d-48e4-b356-61f876c0e612.png)

From above barplot, we can see that student whose gout value is low has
secured good percent of passing grade whereas in fail category students
whose gout value is also low has less percent of failing comparing to
other 4 categories. Furthermore, students whose gout record is high has
also secured good percent of passing grade right after students record
of passing whose gout is medium.

So, from above findings we can say that students who frequently have
outing does have affect in their grades. So, the frequency of students
going out should be reduced.

## 5.8 Does having a romantic relation affect the overall grades of the students?

![image](https://user-images.githubusercontent.com/29594566/178655746-1820652a-389e-4ab1-8ca3-8463b266f40c.png)

As we can see that the students who have romantic status has secured a
smaller number of passing grade compared to students who does not have
any romantic status. And in the failed section we can see that the
students who have romantic status has higher number of fails compared to
students who does not have any romantic status.

So, we can say that having a romantic status for student will affect in
their grades negatively.

