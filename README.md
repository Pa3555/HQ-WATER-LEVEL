# Hydro-Québec Live Dam Data Dashboard (SIUCQ Project)

This project is an experimental **live data web page** designed to display **Hydro-Québec open data** about **dam discharge (flow rate)** and **water level** in real time.  
It’s being developed to support the **SIUCQ (Service d’Intervention d’Urgence Civil du Québec)** teams by providing quick access to **live hydrological data** for **Centre-du-Québec**, especially around **Drummondville**.

---

## Summary

The goal is to:
- Connect to Hydro-Québec’s **open data API**.  
- Retrieve live measurements such as:
  - **Water discharge (débit d’eau)**  
  - **Water level (niveau d’eau)**  
  - **Station information** (name, location, river, etc.)
- Add a **default Centre-du-Québec region filter** shared by both station discovery and record retrieval.  
- Request Hydro-Québec aggregates and records refined by region so that **Drummondville observations are prioritized**.  
- Display all this information on a **live, auto-updating static web page**.

---

## Technical Overview

- Client-side JavaScript (no backend yet).  
- Data source:  
  - [`donnees-hydrometeorologiques`](https://donnees.hydroquebec.com/explore/dataset/donnees-hydrometeorologiques/api/)  
- Hosting target: **Vercel** (static hosting).  

The plan is to fetch and display live JSON data directly from Hydro-Québec’s API, with automatic refresh and regional prioritization.

---

## Current Status

⚠️ I **really need help** getting this to work correctly.

I’m currently facing issues with:
- Receiving and parsing the API responses.  
- Applying proper filters (region, station names).  
- Displaying and refreshing the live values on the web page.  

Right now, the web page is static — it doesn’t yet show live data.

If you have experience with **JavaScript fetch APIs**, **open data integration**, or **client-side live dashboards**, any guidance or contribution would be incredibly appreciated.

---

## Testing

- **Not yet functional** (static prototype).  
- No backend or live refresh currently.  
- Next steps involve connecting the fetch function and auto-refresh logic.

---

## Planned Features

- Live data refresh every few minutes.  
- Regional filters for **Centre-du-Québec**.  
- Graphs and tables showing real-time discharge and water levels.  
- Highlight Drummondville and nearby stations automatically.  
- Future integration with SIUCQ emergency dashboards.

---

## Credits

Developed by **P-A L.**  
Volunteer and Project Manager – **SIUCQ Drummondville**  
Focused on improving real-time situational awareness for emergency response.

---

### Data Source

Hydro-Québec Open Data Portal  
[https://donnees.hydroquebec.com](https://donnees.hydroquebec.com)

