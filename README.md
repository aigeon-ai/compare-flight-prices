markdown
# Compare Flight Prices MCP Server

## Overview

The **Compare Flight Prices** MCP server allows users to compare live flight prices across multiple popular travel sites, including Expedia, Travelocity, Orbitz, Kayak, Priceline, Hotwire, CheapOAir, OneTravel, Vayama, FlightHub, and SkyScanner. This server provides a convenient way to gather real-time flight pricing information, helping users make informed decisions about their travel plans.

## Features

- **Real-Time Price Comparison**: Access live data from multiple travel sites to compare flight prices.
- **Comprehensive Search Parameters**: Customize your search with detailed parameters, including departure and destination cities, travel dates, passenger details, and preferred cabin class.
- **Flexible Flight Types**: Choose between one-way and round-trip flight options.
- **Diverse Cabin Classes**: Compare prices across different cabin classes such as economy, business, first, and premium economy.

## Pricing Plans

- **BASIC**: Free usage with a limit of 1 request per second.
- **PRO**: $19.99 per month.
- **ULTRA**: $49.99 per month.
- **MEGA**: $129.99 per month.

## How It Works

The MCP server operates through two main tools:

### 1. StartFlightSearch

- **Functionality**: Initiates a live search for flight prices across up to 10 sites.
- **Output**: Returns a `SearchID` that can be used to retrieve price data.
- **Parameters**: This tool requires several parameters, including:
  - Departure and return dates (optional for one-way flights)
  - Departure and destination city IATA codes
  - Passenger details (adults, seniors, youth, children, infants)
  - Flight type (one-way or round-trip)
  - Cabin class (economy, business, first, premium economy)

### 2. GetPrices

- **Functionality**: Retrieves gathered flight prices using the `SearchID` from the `StartFlightSearch` tool.
- **Parameters**: Requires the `SearchID` to fetch results.

## Usage Details

### Parameters Overview

- **Flight Type**: 
  - `1` for one-way
  - `2` for round-trip
- **Cabin Class**:
  - `1` for economy
  - `2` for business
  - `3` for first
  - `5` for premium economy
- **Passenger Counts**: Enter the number of passengers for each category (adults, seniors, youth, children, infants) with valid ranges from 0 to 9.

## Conclusion

The Compare Flight Prices MCP server is a versatile tool designed to simplify the process of searching for and comparing flight prices. By utilizing its comprehensive features and real-time data capabilities, users can efficiently plan their travel while accessing competitive pricing from leading travel websites.