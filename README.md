# Baltimore-City-Public-School-Kindergarten-Readiness-Assessment

## Background
[Kindergarten readiness](https://www.unitedway.org/blog/kindergarten-readiness-why-is-it-important#:~:text=The%20first%20few%20years%20of,%2C%20counting%2C%20and%20social%20interaction.) influences the academic success of students because foundational academic and social skills improve their abilities to adapt and flourish in new school environments. Reading, writing, and math skills would enable students to understand new concepts more easily, and strong social interaction capabilities would facilitate cooperation with peers. However, there are discrepancies in kindergarten readiness due to different socioeconomic backgrounds, forms of prior care, and levels of language fluency. Students who are economically disadvantaged, lack prior care, or are non-native English speakers face greater challenges in achieving readiness for kindergarten curriculums. This analysis seeks to understand what solutions Baltimore City Public Schools should implement to address those concerns. 

Baltimore City has already invested in early learning programs like [Judy Centers](https://earlychildhood.marylandpublicschools.org/families/judy-centers) that provide pre-kindergarten classrooms, child care assistance, developmental and health screenings, family enagement activities, parenting classes, and play groups. The Judy Centers address the needs of both students and families to provide multiple forms of support in a child's academic and social development. Comparing the impact of Baltimore City early learning programs with traditional child care centers, home care, or other public settings could generate insights into the successes, challenges, and strategies for improvement. 

A member of our team also tutors an elementary school student from Baltimore City through the Johns Hopkins Tutorial Project, so the insights from this analysis could potentially provide more context about the school system. 

## Business Question
How should Baltimore City allocate resources to improve kindergarten readiness for its public schools? 

## Data Question - Open Data
This analysis uses data from [Baltimore City Public Schools](https://www.baltimorecityschools.org/data) about student achievement. We wanted to analyze the preparation of students entering Baltimore City Public Schools, so we explored districtwide results for the Maryland State Department of Education Kindergarten Readiness Assessment in 2019-2020. Students take the exam early in their kindergarten year and receive scores on math, language arts, social development, and physical well-being. In contrast to other Maryland counties that only administered the exam to small samples, Baltimore City tested all kindergarten students.

### The dataset includes the following for each school and student group: 
- Test Takers With Overall Score
- Average Scale Score
- Average Language and Literacy Score
- Average Math Score
- Average Physical Development Score
- Average Social Foundations Score
- Percent Emerging Readiness
- Percent Approaching Readiness
- Percent Demonstrating Readiness

### The student groups (with definitions from the dataset) are the following: 
- All students
- Economic Disadvantaged
- English Learners
- Gender
- Race
- Prior Care: 
  - **Baltimore City Public Schools Pre-K With Judy Center**
  - **Baltimore City Public Schools Pre-K Without Judy Center**
  - **Head Start:** A federal preschool program for children from low-income families
  - **Child Care Center:** Child care provided in a facility, usually non-residential, for part/all of the day that provides care to children in the absence of the parent
  - **Family Child Care Center:** Regulated care given to a child younger than 13 years old, in place of parental care for less than 24 hours a day, in a residence other than the child’s  residence and for which the provider is paid
  - **Informal Care:** Care by parent(s) or a relative
  - **Non-Public Nursery School:** Preschool programs with an education focus for 3-4 year olds that is part-day and occurs nine months a year.
  - **Repeated Kindergarten:** The student was enrolled in kindergarten in the prior school year
  - **Unknown:** The student did not have a prior care setting recorded in the official test file from Maryland State Department of Education
  - **Other Pre-K**

## Data Question - Analysis
This analysis uses Microsoft Excel to answer the following questions:
- How prepared are kindergarten students who enter Baltimore City Public Schools in math, language and literacy, physical development, and social foundations? How do results differ from students who are economically disadvantaged, non-native English speakers, and have different types of prior care?
- How can we group Baltimore City Schools based on the readiness of their kindergarten students?

## Data Answer
### Pivot Tables
Pivot tables produced the following graphs illustrating the average scores for children with different forms of prior care. A clear pattern emerges because informal care has the lowest average scale, language and literacy, math, physical development, and social foundations scores. Across all areas, the scores then gradually increase for prior cares in the following order: Family Child Care Centers, Other Pre-Ks, Head Starts, Child Care Centers, Baltimore City Public Schools Pre-Ks without Judy Centers, Baltimore City Judy Center Judy Center Pre-Ks, and non-public nursery schools. 

#### Pivot Chart 1 - Average Scale Score by Type of Prior Care
![alt text](https://github.com/Daphne-Tang/Baltimore-City-Public-School-Kindergarten-Readiness-Assessment/blob/main/Screenshots/Average%20Scale%20Score%20By%20Type%20of%20Prior%20Care.png)

The following two graphs demonstrate the scores for economically disadvantaged students and English Learners. Both student groups tend to be stronger in physical development and social foundations but are lacking in language and literacy and math skills. 

#### Pivot Chart 2 - Average Scores for Economically Disadvantaged Students
![alt text](https://github.com/Daphne-Tang/Baltimore-City-Public-School-Kindergarten-Readiness-Assessment/blob/main/Screenshots/Average%20Scores%20for%20Economically%20Disadvantaged%20Students.png)

#### Pivot Chart 3 - Average Scores for English Learners
![alt text](https://github.com/Daphne-Tang/Baltimore-City-Public-School-Kindergarten-Readiness-Assessment/blob/main/Screenshots/Average%20Scores%20for%20English%20Learners.png)

### Cluster Analysis
Cluster analyses show how Baltimore Public Schools can be grouped in terms of 1) readiness 2) physiosocial development. The following tables show two 3x-cluster analyses for kindgergarteners at Baltimore Public Schools. The first is based on readiness: Percent Emerging Readiness, Percent Approaching Readiness, and Percent Demonstrating Readiness. The second is based on physiosocial development: Average Language and Literacy Score, Average Math Score, Average Physical Development Score, and Average Social Foundations Score. 

#### Cluster 1 - Readiness
![alt text](https://github.com/Daphne-Tang/Baltimore-City-Public-School-Kindergarten-Readiness-Assessment/blob/main/Screenshots/cluster%20readiness.png) 

In this analysis:
- Cluster 1 "Low Readiness" (Count: 26) 
  - Anchored to Westport Academy
  - High in emerging readiness, below average in approaching and demonstrating readiness
- Cluster 2 "High Readiness" (Count: 28)
  - Anchored to Woodhome Elementary/Middle School
  - High in demonstrating readiness, below average emerging and approaching readiness
- Cluster 3 "Medium Readiness" (Count: 58)
  - Anchored to Garrett Heights Elementary/Middle School
  - Above average approaching readiness, slightly above average emerging readiness, below average demonstrating readiness

Approximately 50% of schools fall into the "Medium Readiness" category, whereas the other 50% of schools are split relatively evenly amongst "Low Readiness" and "High Readiness" clusters. 

#### Cluster 2 - Physiosocial Development
![alt text](https://github.com/Daphne-Tang/Baltimore-City-Public-School-Kindergarten-Readiness-Assessment/blob/main/Screenshots/cluster%20physiosocial%202.png)

In this analysis:
- Cluster 1 "Low Physiosocial Development" (Count: 12) 
  - Anchored to Guilford Elementary/Middle School
  - Well below avaerage in language/literacy, math, physical development, and social foundations scores 
- Cluster 2 "Medium Physiosocial Development" (Count: 63)
  - Anchored to Furman Templeton Prepatory Academy
  - Slightly below avaerage in language/literacy, math, physical development, and social foundations scores 
- Cluster 3 "High Physiosocial Development" (Count: 36)
  - Anchored to Dorothy I. Height Elementary School
  - Above avaerage in language/literacy, math, physical development, and social foundations scores 

Approximately 50% of schools fall into the "Medium Physiosocial Development" category. About 12.5% of schools are in the "Low Physiosocial Development" cluster and about 37.5% in the "High Physiosocial Development" cluster. In other words, about two thirds of Baltimore Public Schools are in clusters that represent below average physiosocial development. 

#### Cluster Visualization 1 -

#### Cluster Visualization 2 - 

## Business Answer
Based on results from the Kindergarten Readiness Assessment, students receiving informal care from parents or relatives often have the lowest scores across all areas, including language and literacy, math, physical development, and social foundations. Non-public nursery schools have the highest scores, but Baltimore City School Pre-Ks, especially Judy Centers, are close behind. These findings indicate that the Baltimore City Public School System could expand access to their Pre-Ks, particularly for children who are economically disadvantaged and non-native English speakers. The city could also conduct a geographic analysis to identify the locations where children do not have access to prior care and strategically open Judy Centers or city-sponsored programs in those areas. These initiatives would require more funding and resources, but the outcome would be impactful: greater kindergarten readiness would allow students to easily adapt to new school environments in both academics and social interactions with peers. However, the plans outlined above could also help Baltimore City Public Schools conserve resources by making more targeted investments. With the COVID-19 environment, Baltimore City Public Schools could also consider bolstering the online components of their prior cares to sustain the impact of their programs. 

Furthermore, the Baltimore City Public Schools could create a forum where representatives of different prior cares would discuss best practices in enhancing kindergarten readiness. After administrators and teachers share their successes, challenges, and strategies, the implementation of best practices in family child care centers, head starts, child care centers, Baltimore City Public Schools Pre-Ks (including Judy Centers) could potentially decrease the discrepancies in kindergarten readiness across different forms of prior care. Baltimore City Public Schools could also consider developing and strengthening online resources or webinars to assist parents or family members with informal care such that their strategies align with curriculums in Pre-Ks. This would bolster the kindergarten readiness of children that cannot attend prior care due to financial, geographic, or time constraint reasons. 

If prior cares have economically disadvantaged students and non-native English speakers who tend to have lower language and literacy and math scores, they could dedicate more resources to breaking down the knowledge gap or language barriers. 
