# BioSTL Atlas: St. Louis Biotech Company Database

This repository hosts a simple web-based database of biotech companies in the St. Louis area for BioSTL.  
The website reads directly from a CSV file and automatically displays:

- A searchable/filterable company table  
- An interactive map showing company locations  

No coding is required to update the data — you only need to edit the CSV file.

---

## How the Website Works

The website loads company data from a single file:

DataCompany.csv

Every time this CSV is updated and pushed to GitHub, the website updates automatically.

---

## CSV Format

Each row in the CSV represents one company.

### Required Columns

The CSV must contain the following columns in this exact order:

| Column Name |
|------------|
| Company Name |
| Company Type |
| Industry Sector |
| Brief Description |
| Location (County) |
| Location |
| Website |
| LinkedIn Profile |
| Employees |
| Latitude |
| Longitude |

---

## Adding or Editing Companies

To update the database:

1. Open DataCompany.csv  
2. Edit, add, or delete rows  
3. Save and commit the file  

That’s it — the website will reflect the changes.

---

## Multiple Locations for One Company

If a company has multiple locations, list them in the same row by separating values with a semicolon `;`.

Example:

Location:  
...St. Louis, MO; ...Chesterfield, MO  

Latitude:  
38.6270; 38.6631  

Longitude:  
-90.1994; -90.5771  

Make sure:

- The number of locations matches the number of latitudes and longitudes.  
- They are in the same order.

---

## Map Coordinates

Latitude and Longitude must be in decimal format:

- Latitude: between -90 and 90  
- Longitude: between -180 and 180  

You can find coordinates using Google Maps:

1. Right-click on a location  
2. Click the coordinates to copy them  

---

## Replacing the Domain Name

If you deploy this site under your own domain, replace:

danibocsi.github.io

with your new domain wherever it appears in the project.

---
