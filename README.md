# Hydro-Québec Live Dam Data Dashboard (SIUCQ Project)

This project is an experimental **live data web page** designed to display **Hydro-Québec open data** about dam conditions — specifically **water discharge (flow rate)** and **water levels** in real time.  
The purpose is to support **SIUCQ (Service d’Intervention d’Urgence Civil du Québec)** teams with rapid access to hydrological data for **Centre-du-Québec**, including the **Drummondville** area.

---

## Summary

This project attempts to:
- Connect to **Hydro-Québec’s open data API**.  
- Retrieve live measurements such as:
  - **Water discharge (débit d’eau)**
  - **Water level (niveau d’eau)**
  - **Station metadata** (location, name, river, etc.)
- Apply a **default region filter** for **Centre-du-Québec** so that Drummondville stations appear first.  
- Display all this information on a **public, auto-updating static web page** for emergency monitoring.

---

## Technical Notes

- The app uses **client-side JavaScript (fetch API)** to request Hydro-Québec datasets.  
- API endpoints:  
  - [`donnees-hydrometeorologiques`](https://donnees.hydroquebec.com/explore/dataset/donnees-hydrometeorologiques/api/)  
  - [`evenements-pointe`](https://donnees.hydroquebec.com/explore/dataset/evenements-pointe/api/) (for extra data when available)
- Intended deployment: **Vercel** (static hosting with live API calls).  

---

## Challenges

I’m currently working through:
- Fetching and parsing Hydro-Québec’s JSON data correctly.  
- Managing rate limits and API query parameters.  
- Keeping the data display **live and automatically refreshed** without needing a backend.  

The goal is to show **real-time dam and river status** for use by emergency response teams during critical events such as **flooding** or **ice break-up**.

---

## Testing

- Not yet fully functional — only static test pages.  
- No backend processing (client-only).  
- Next phase: integrate real API calls and dynamic updates on the page.

---

## Next Steps

- Implement region-based filtering (`Centre-du-Québec`).  
- Fetch live discharge and level data from all available Hydro-Québec stations.  
- Highlight Drummondville and nearby sites automatically.  
- Add chart visualizations for live readings (flow rate & level).  
- Deploy and test through Vercel hosting.

---

### Credits

Developed by **P-A L.**  
Project: **SIUCQ Drummondville – Live Hydro Monitoring Dashboard**  
For civil protection and emergency response readiness.

---

### Data Source

Hydro-Québec Open Data Portal  
[https://donnees.hydroquebec.com](https://donnees.hydroquebec.com)
