# geofeed
About
This project implements the RFC 9632 specification for creating and validating Geofeed files. Geofeeds allow network operators to publish geolocation information for their IP prefixes in a standardized way.
What is a Geofeed?
A Geofeed is a CSV file that associates IP prefixes (IPv4 and IPv6) with geographic locations. It enables:
Improved IP geolocation accuracy
Reliable geographic data for third-party services
Compliance with data localization regulations
Optimized content delivery (CDN)
 File Format
According to RFC 9632, a Geofeed file follows this format:
# Geofeed Version 1.0
# https://example.com/geofeed.csv
192.0.2.0/24,US,US-CA,Los Angeles,90001
2001:db8::/32,FR,FR-IDF,Paris,75001
1
2001:db8::/32,FR,FR-IDF,Paris,75001
Structure
IP Prefix: CIDR notation (IPv4 or IPv6)
Country Code: ISO 3166-1 alpha-2
Region: ISO 3166-2 (optional)
City: City name (optional)
Postal Code: Postal code (optional)
 RFC 9632 Specifications
CSV format with UTF-8 encoding
IPv4 and IPv6 support
Comments starting with #
Optional fields for region, city, and postal code
ISO 3166 code validation
Optional RPKI signature
 Resources
RFC 9632 - Finding and Using Geofeed Data
IANA Geofeed Registry
ISO 3166 Country Codes
 License
MIT License - see the LICENSE file for details.