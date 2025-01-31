# Sales Fill Rate Report Extension for D365 F&O

## Overview
This extension adds a Sales Fill Rate Report to D365 Finance and Operations, allowing users to analyze order fulfillment rates and delivery performance. The report is accessible through Sales & Marketing > Inquiries > "Sales Fill Rate Report".

## Features
- Calculate fill rates based on ordered vs shipped quantities
- Track backorder quantities
- Analyze delivery performance (promised vs actual dates)
- Filter by customer, site, and sales unit
- Support for customer hierarchy filtering
- Performance optimized for large datasets (500k+ sales lines)

## Technical Details
- Model Name: RSMSalesFillRate
- Publisher: RSM
- Version: 1.0.0.0
- Layer: 50 (ISV)

## Installation
1. Import the model file into your D365 environment
2. Synchronize the database
3. Grant appropriate security privileges to users

## Security
The extension includes the following security privileges:
- `rsmSalesFillRatePrivilege`: Allows users to view and run the Sales Fill Rate Report

## Dependencies
- Base D365 F&O application
- Sales and Marketing module

## Usage
1. Navigate to Sales & Marketing > Inquiries > Sales Fill Rate Report
2. Select the date range (required)
3. Optionally filter by:
   - Customer Account
   - Site ID
   - Sales Unit
4. Run the report to view results

## Performance Considerations
- Uses in-memory temporary tables for optimal performance
- Implements efficient query patterns
- Includes appropriate indexing
- Designed to handle 500k+ sales lines under 3 seconds

## Support
For support, please contact your RSM representative or open an issue in this repository. 