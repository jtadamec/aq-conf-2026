# Aquarius Conference 2026 

## Glossary 
- **DRT** - Data Review Tool 

## Feature Enhancements 2025

- AQ Time Series
  - out of sequence or duplicated data can now be imported
    - ignores duplicates and non-sequential when selected
  - DRT Gap Fill
    - Default behavior should match the gap tolerance for an individual time series 
- HydroCorrect (what is this)
  - Alert Management
    - Aggregation
    - Acknowledge (instead of approve)
      - how does this relate to what OD would be doing with alerts? 
  - Filtering options
    - rule type
    - alert type 
    - type of time series
  - Audit rule modification
- WebPortal 
  - Take location notes visible in time series able to be viewable in web portal through a chart 
  - Email Settings (do we do anything with notifications yet)
    - replyto email header, display name for recipients
  - Security improvements 
    - Define activity limits to log users off after X amount of time
  - Support resources aggregated (same as time series)
  - Synchronizing extended attributes 
    - When synced from time series to AQWP they are syn
  - Store basemap credentials 
    - Can be stored as a global setting for a basemap 

## Future Enhancements

- Samples
  - Mapping for data fields so that input can be added without conforming specifically to Samples format 
  - Integration with Time-Series and Web Portal 
    - Design phase 
    - More metadata from samples should be available to web portal consumers 
  - Improving integration with external systems 
    - Support the use of externally generated GUIDs and sample names
    - Fields can be brought into samples to have a cross reference across multiple systems 
- Time-Series
  - Support calculation of moving averages built into derived TS
    - "What is the precipitation level over the past 7 days" 
  - Assign a sensor to a time series in DRT
    - Goal is to be able to pull the accuracy from the sensor and have it be represented in DRT as an uncertainty bound 
    - Data would be available in an API 
    - Currently able to be assigned to a location only?
  - Support for QRevMS file formats
- HydroCorrect 
  - Automatic estimation using a surrogate time series (2026.1)
    - Automate the process of estimating bad or missing data 
    - Based on data from one time series it will estimate the gap correction for the flawed one 
  - Aggregated alerts and bulk undo 
  - Improvements to rule tuner for UI improvements 
  - User will be able to write custom rules (design discussions only currently)
- Web Portal 
  - Define the ordering of dashboards (2026.1) 
    - Currently alphabetic only
    - Admins will be able to drag them into the orders that they should be seen 
  - AA WCAG accessibility support for public facing pieces 
  - Samples metadata being available in Web Portal 
  - Visitor analytics (via google analytics) to track site usage
    - Umami (GDPR compliant) also available 
- Connect 
  - Token based authentication 
    - currently only supports credentials
  - Communicating export failures 
  - Improved file processing around "next start point" value

  ![Future Timeline](/resources/future-enhancements.jpg)