# Tourism-management-system
A MySQL database for managing tourist spots, hotels, restaurants, tour guides, and local culture information.


# Tourist Spot Management System - Database

This repository contains the MySQL/MariaDB database dump for the **Tourist Spot Management System**, exported via phpMyAdmin.

## Database Overview

The database stores information related to tourist destinations, including:

- **division** / **district** – administrative divisions and districts
- **famous_place** – tourist spots with location and fun facts
- **famous_person** – notable people associated with places
- **local_culture** – cultural highlights, local food, and language by district
- **environmental_effect** – environmental issues and traveler impact tips
- **suitable_season** – best seasons and activities for each place
- **hotel** / **restaurant** – accommodation and dining options near tourist spots
- **tour_guide** / **photographer** – service providers with contact info, ratings, and rates
- **visitors** – annual visitor statistics and ratings

## Files

| File | Description |
|------|--------------|
| `tourist_spot_management_system.sql.gz` | Compressed SQL dump (recommended for download) |
| `tourist_spot_management_system.sql` | Uncompressed raw SQL dump |

## Requirements

- MySQL 5.7+ or MariaDB 10.4+
- phpMyAdmin (optional, for GUI import)

## How to Import

### Option 1: Using the MySQL/MariaDB command line

```bash
# If using the compressed file
gunzip -k tourist_spot_management_system.sql.gz

# Create a database (if not already created)
mysql -u root -p -e "CREATE DATABASE tourist_spot_management_system;"

# Import the SQL file
mysql -u root -p tourist_spot_management_system < tourist_spot_management_system.sql
```

### Option 2: Using phpMyAdmin

1. Create a new database.
2. Go to the **Import** tab.
3. Choose `tourist_spot_management_system.sql` (or the `.gz` file directly — phpMyAdmin supports gzip uploads).
4. Click **Go**.

## Notes

- This dump was generated with `phpMyAdmin 5.2.1` on `MariaDB 10.4.32`.
- No credentials or sensitive personal data are included in this dump.
- Feel free to open an issue or pull request for corrections or improvements to the schema/data.

## License

Add your preferred license here (e.g., MIT).
