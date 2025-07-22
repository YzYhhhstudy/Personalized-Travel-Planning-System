# Personalized Travel Planning System
<img width="586" height="499" alt="image" src="https://github.com/user-attachments/assets/493973b2-544e-4bee-b61d-1e54927b0f74" />



## Agencies Involved
- **Travel Planner**
- **Travel Q&A Agency**

## Mind Stream
[![Mind Stream](https://github.com/user-attachments/assets/cfe46c63-6df1-46fa-a05d-acf5dce9822e)](https://github.com/user-attachments/assets/cfe46c63-6df1-46fa-a05d-acf5dce9822e)

## Interface
### Travel Planner
- **Input**
  ![Travel Planner Input](https://github.com/user-attachments/assets/32edc71b-266d-4758-af2c-511355fb55fc)

- **Output**
  ![Travel Planner Output](https://github.com/user-attachments/assets/204dd3bd-d040-46c8-a669-8483a3754595)

### Travel Q&A Agency
- **Weather Search**
  ![Weather Search](https://github.com/user-attachments/assets/0c092960-96df-4e69-8bb5-db05c2cf9fca)

- **Neighborhood Search**
  ![Neighborhood Search](https://github.com/user-attachments/assets/a682fa31-04b9-464b-8756-a7b890b9b671)

- **Networking Search**
  ![Networking Search](https://github.com/user-attachments/assets/67c0f4d1-14d1-4a2e-b087-03a2d99feed3)

- **Recommended Activities**
  ![Recommended Activities](https://github.com/user-attachments/assets/06f44fb0-b28f-4cb8-b3d4-a38dbf5ce262)

## Analysis
### Backend
- **get_location_data(location, api_key)**: 
  - Using Qweather API, input location (name or geocode) and API key to generate JSON data.
  
- **get_weather_forecast(location_id, api_key)**: 
  - Using Qweather API, input location ID or Lat and Lng to generate a 3-day weather forecast.
  
- **get_geocoding(input_address)**: 
  - Using Google Maps API, input the address to generate Lat and Lng.
  
- **get_recommendation(input_address)**: 
  - Using Google Maps API, input the address to generate restaurant recommendations within a 1500m radius.
  
- **get_shopping_mall(input_address)**: 
  - Using Google Maps API, input the address to generate shopping recommendations.
  
- **process_network(input_question)**: 
  - Using OpenAI API to generate responses for the input question.
  
- **Exp_what_2_play(destination, departure_date, back_date)**: 
  - Searching on Expedia.com to generate a link showing activities for the specific trip.
  
- **chat_with_gpt(chat_destination, chat_history, chat_departure, chat_departure_date, chat_back_date, chat_style, chat_budget, chat_people, chat_other)**: 
  - Using OpenAI GPT-4, given prompts using those inputs, GPT will generate trip recommendations.

### Frontend
- Gradio
- CSS
- HTML

## Preparation
### Requirements
- os
- openai
- gradio
- requests
- googlemaps
- HTML

### APIs
- **Qweather**: For weather info and forecasts
- **OpenAI**: The main helper
- **Google Maps**: For recommendations in specific locations

## Version History
### V1 - V2
- Built foundational framework
- Basic travel planning functionality

### V3 - V4
- Added more functions
- Defined our logo

### V5 - V6
- Developed the Travel Q&A agency
- Final version, fixed some bugs
