Propsal
Buisness context: Describe what you are making and what it does

Functional Requirements
  Homepage- eg. Describe what is on it is data input required, what buttons do.
  Navbar- what its in it
  About pages- whats described on them

Non functional
  Security
  Maintainability
  Performance
  Usability
  Accessibility

Decomposition
  A little bulletpointed of pages to summarise whats on them

KPIS
  User Engagement:
  Daily Active Users
  Average Session Duration
  User Retention Rate - Returning users
  Bounce Rate - Percentage of users who leave after veiwing one page
  Number of Users Tracking Energy Usage
  Number of Consultations/Instalemtns Booked
Hardware and software 
  Ai chatbot
  Payments on website

ERD
User  
PK  UserId  
    Username  
    Password  
    Email  

EnergyUsage  
PK  UsageId  
FK  UserId  
    Date  
    EnergyConsumed_kWh  
    SolarGenerated_kWh  

CarbonFootprint  
PK  FootprintId  
FK  UserId  
    Date  
    CO2Emissions_kg  

InfoPage  
PK  PageId  
    Title  
    Content  

Calculation  
PK  CalcId  
FK  UserId  
    Type  
    Result  
    Date  

User → EnergyUsage (1-to-Many)
User → CarbonFootprint (1-to-Many)
User → Calculation (1-to-Many)
Calculation → CarbonFootprint (Many-to-1)
User → InfoPage (Many-to-Many, if users can bookmark pages)
