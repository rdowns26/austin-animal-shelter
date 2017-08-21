# austin-animal-shelter
We explored what characteristics lead to higher adoption rates, and built a model to predict the likelihood of adoption

**This project was done by Rachel Downs, Mitchell Kagel, Arti Kumar, Juan Ramos, and Mario Luevano for an MIS elective at UT Austin.**

## Project Goals:
We are analyzing a dataset of intakes and outcomes from Austin Animal Shelter to understand animal adoption trends, including which attributes of animals result in a higher likelihood of adoption. Our final goal is to predict whether or not an animal will be adopted based on characteristics Austin Animal shelter can identify upon intake.

This problem is important because according to the ASPCA, [6.5 million animals enter animal shelters each year](https://www.aspca.org/animal-homelessness/shelter-intake-and-surrender/pet-statistics). Furthermore, each year 1.5 million shelter animals are euthanized. We chose this problem because as Austin continues to grow and continue to be a pet-friendly city, naturally the number of animal intakes will continue to increase and [the Austin Animal Shelter is already experiencing tumult from having to turn away animals](http://www.mystatesman.com/news/local/crowded-austin-animal-shelter-has-turned-away-some-healthy-dogs-cats/vUw1yYwPeLDHpw44cU066K/). To avoid this problem, the shelter is able to transfer animals to other shelters, partner with fosters, and other mechanisms. We hope our analysis will provide detailed insight into the leading factors of whether an animal will be adopted or not to inform the operations of the Austin Animal Shelter.

## Data Processing:
We used datasets of Austin Animal Shelter intakes and outcomes found on http://data.austintexas.gov. We performed the following steps to clean our data and extract the features needed for our analysis and model:
- Performed an inner join on intakes/outcomes datasets on Animal ID
- Extracted the gender and spayed/neutered status for each of the intake and outcome columns
- Calculated duration of stay, placed animals in “age buckets” and “duration buckets” to simplify analysis of these continuous variables
- Created boolean fields for specific breed terms (i.e. pit bull chihuahua mix would be given a 1 in both the pit bull and chihuahua columns)

## [Read Our Project Report](https://data.world/rdowns26/austin-animal-shelter/file/Project%20Report.pdf)

Austin Animal Center Intakes: [Source](https://data.austintexas.gov/Health/Austin-Animal-Center-Intakes/wter-evkm)

Austin Animal Center Outcomes: [Source](https://data.austintexas.gov/Health/Austin-Animal-Center-Outcomes/9t4d-g23)
