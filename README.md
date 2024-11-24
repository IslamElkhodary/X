# Digital Egypt Pioneers Initiative - DEPI

## Project Report
[Download Project Report](https://drive.google.com/file/d/1h2lQ3r8rUnp219uLdxOfSCnX85RrbVQ1/view?usp=sharing)

## Table of Contents
1. [Additional Columns](#additional-columns)
2. [Assumptions and Remarks](#assumptions-and-remarks)
3. [Data Status](#data-status)
4. [Demand Loss (MW)](#demand-loss-mw)
5. [Event Type](#event-type)
6. [Detailed Event Type](#detailed-event-type)
7. [Cleaning Steps](#cleaning-steps)
8. [Key Performance Indicators (KPIs)](#key-performance-indicators-kpis)

## Additional Columns
We added some columns to enhance the dataset, providing more detailed insights into the power outage events. These new columns are:

- **Duration Time**: Captures the duration of the outage, calculated by subtracting the Date Event Began from the Date of Restoration.
- **Detailed Event Type**: Provides more specific information about the event categories.
- **Data Status**: Indicates the type of data, categorized as Faulty, Anonymous, Full, or Fair.
- **Years Group**: Organizes the data into specific year ranges (e.g., 2002-2010, 2011-2014).

## Assumptions and Remarks
### Date and Time
The time 5:78 PM in the 2005 sheet was identified as a typographical error. The following conversions were made:
- Evening: 6:00 PM
- Noon: 12:00 PM
- Midnight: 12:00 AM

In cases where the date and time of restoration are unknown and the Demand Loss (MW) is recorded as zero, we assumed that the electric current was restored simultaneously.

### Data Status
- **Faulty**: Power outage duration exceeds one hour with zero demand loss.
- **Anonymous**: NULL values for the number of customers affected and demand loss.
- **Full Data**: Complete entries for key metrics.
- **Fair Data**: Partially complete entries.

## Demand Loss (MW)
Assumed that "none" is equivalent to zero. For calculations:
- Average household consumption: 1.2 kWh/hour.
- Outage duration: Difference between Time Event Began and Time of Restoration.
- Number of individuals per household: Assumed to be 3.

We used AI to calculate demand loss for specific records based on predefined assumptions.

## Event Type
In the 2023 sheet, "Public Appeal" is considered equivalent to "Shedding Load".

## Detailed Event Type
Categorizes
