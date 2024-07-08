# PPP_loan_analysis
## Analysis of the PPP Loans that were issued to Small Businesses during COVID-19

By Jose Garcia, Erika Chunzho and Gelbert Ramos

## Table of Contents:
1) Business Problem
    Context and Business Problem
    Business Requirements
    Functional Requirements
2) Business Impact
3) Business Persona
4) Data
5) Methods
    Information Architecture Diagram
    Data Architecture Diagram 
    Technical Architecture Diagram
    Data Pipelines/ ETL/ELT Diagram
    Dimensional Modeling Diagram
6) Data Tools
7) Interface

## Business Problem

#### Context and Business Problem
    During the COVID-19 pandemic, the U.S. government established the Paycheck Protection Program (PPP). The program provided loans to small businesses to help them maintain their workforce during the pandemic. Most loans were forgivable if used primarily for payroll and other specified business expenses like utilities.

    The PPP was designed to provide rapid financial assistance to small businesses nationwide. However, this rapid deployment raised concerns about the program's effectiveness and equitable distribution of funds. The PPP faced several challenges, including eligibility issues, fraud, and disparities in loan distribution among different demographic groups and geographic areas.

### Business Requirements
#### The primary business problems this analysis aims to address are:
1. Measuring and Analyzing the Distribution of PPP Loans:
    * Calculate the total loan amounts disbursed by state, industry, and company.
2. Identifying Geographic Areas or Industries That May Have Been Underserved or Overserved:
    * Analyze the distribution of PPP loans across different states, counties, and zip codes to identify geographic disparities.
3. Assessing the Effectiveness and Impact of the PPP Loan Program:
    * Evaluate how well the PPP loans supported business survival and recovery during the COVID-19 pandemic.

#### Key Performance Indicators (KPIs):Establish metrics for business success
1. Loan-to-GDP Ratio: Measures the proportion of PPP loans relative to the economic output of counties and states.
    * Ratio to compare the total loan amount allocated vs GDP by county and states
    * (Total Loan Amount / GDP) * 100
2. Industry Impact Ratio: Compares the proportion of loans given to an industry relative to its economic contribution.
    * (Loan Amount to Industry / Total Loan Amount) / (Industry GDP / Total GDP)
3. Rural vs. Urban Loan Allocation: Assesses the balance of loan distribution between rural and urban areas.
    * (Rural Loan Amount / Total Loan Amount) / (Rural Population / Total Population)

### Functional Requirements 
#### Business Intelligence Use Cases:
1. Analyze PPP loan disbursements by company, industry, geography
2. Monitor loan amounts and number of businesses assisted by lender
3. Report on top lenders, industries, and geographic areas based on loan portfolios
4. Analyze the correlation between PPP loans and economic indicators like GDP
 
### Requirements:
    1. Must have
        a. Total loan by companies
        b. Total loan by State
        c. Total Business by States
        d. Top 10 Lenders by State
        e. Total Loan by Lenders
        f. Classification by NAICS Code
        g. Total amount per industry, PPP, then PPS
        h. Aggregate data based on GDP for the past four years, or COVID-19 per zip code

    2. Should have 
        a. Loan forgiveness amount and rate by state, industry, and lender
        b. Track loan approvals and disbursements over time to identify trends and patterns.
        c. Compare loan distribution between rural and urban areas.

    3. Nice to have
        a. Analyze loan distribution based on Race, Ethnicity, Gender, and Veteran status fields to assess equity in loan allocation.
        b. Calculate and compare the average processing time and approval rates for different lenders.

    4. Forget about it (which could also be future work)
        a. Long-term business performance tracking: Would need access to    ongoing financial data for loan recipients
        Integration with real-time economic indicators
        b. Fraud detection analysis
