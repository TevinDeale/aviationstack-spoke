# AviationStack API Integration Spoke

## Overview
Custom IntegrationHub spoke that retrieves flight data using the AviationStack API, processing flight codes to return detailed flight information.

## Technical Specifications

### Action Details
- Name: Get Flight Details
- Input: Flight Code (string)
- Output: Complex object containing parsed flight data

### API Integration
- Endpoint: AviationStack API
- Authentication: API Key
- Method: GET
- Response Format: JSON

### Data Processing
- Parses JSON response from AviationStack
- Transforms raw data into structured complex object
- Handles API response validation and error cases

### Output Structure
Complex object containing:
- Flight status
- Departure information
- Arrival information
- Airline details
- Aircraft information
- Schedule data

## Implementation Notes
- RESTMessage for API communication
- JSON parsing for response handling
- Error handling for API failures
- Data validation for input/output

## Usage
Called via flow designer to populate flight request forms with validated flight information.
