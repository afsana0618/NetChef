# NetChef – A Network-Based Recipe Aggregator

NetChef is a Python-based tool that fetches recipes from the Spoonacular API and analyzes network traffic to optimize performance. It demonstrates how caching, API monitoring, and traffic inspection can improve real-world app responsiveness and bandwidth efficiency.

## Features

-  Search for recipes using specific ingredients via Spoonacular API  
-  Backend optimized with Redis caching and response compression  
-  Analyze API performance and response times using logged data  
-  Visualize traffic patterns with Pandas and Matplotlib  
-  Capture and inspect network traffic using Wireshark  

## Technologies Used

- **Python**  
- **Flask** – backend logic and routing  
- **Redis** – in-memory caching  
- **Wireshark** – for packet-level traffic inspection  
- **Pandas** – for data analysis  
- **Matplotlib** – for graph generation  
- **dotenv** – for managing API secrets  
- **Spoonacular API** – for recipe data  


## 📸 Sample Visualizations

Created by `visualize_network.py`:
- API usage over time  
- Response time distribution (Lunch vs. Dinner)  
- HTTP status code breakdown  

*Note: Graphs are not included in this repository preview but were part of the final report.*

## 🔐 Security & Resilience

- API key secured via `.env` file (excluded via `.gitignore`)  
- Graceful error handling for:  
  - Missing or invalid ingredient input  
  - Redis connection failures  
  - Spoonacular API exceptions  
- HTTPS used for all external requests to ensure encrypted transmission  

## 🧪 Network Traffic Analysis

We used **Wireshark** to monitor and inspect API requests:
- Tracked HTTP/HTTPS packet sizes  
- Measured bandwidth usage before and after Redis caching  
- Identified any packet retransmissions and inefficient request patterns  

Performance logs (`timings.csv`) were used to evaluate and visualize:
- Cached vs. uncached response times  
- Frequency of API endpoint hits  
- Status code distributions  

## Future Improvements

- Add multi-ingredient search and advanced filtering  
- Integrate multiple recipe APIs for data redundancy  
- Implement adaptive caching strategies  
- Test performance over mobile and cellular networks  

## Team

- **Afsana Halim**  
- **Dina Mansour**  
- **Maisha Hasan**  

## License

This project was created for academic and educational use only.


