Geofeed RFC 8805
A parser and validator for Geofeed files compliant with RFC 8805.
About
This project implements the RFC 8805 specification for creating and validating Geofeed files. Geofeeds allow network operators to publish geolocation information for their IP prefixes in a standardized way.
What is a Geofeed?
A Geofeed is a CSV file that associates IP prefixes (IPv4 and IPv6) with geographic locations. It enables:
Improved IP geolocation accuracy
Reliable geographic data for third-party services
Compliance with data localization regulations
Optimized content delivery (CDN)
 File Format
According to RFC 8805, a Geofeed file follows this format:
Geofeed format as per RFC 8805
192.0.2.0/24,US,US-CA,Los Angeles
2001:db8::/32,FR,FR-IDF,Paris
Structure
IP Prefix: CIDR notation (IPv4 or IPv6)
Country Code: ISO 3166-1 alpha-2
Region: ISO 3166-2 (optional)
City: City name (optional)
 RFC 8805 Specifications
CSV format with UTF-8 encoding
IPv4 and IPv6 support
Comments starting with #
Optional fields for region and city
ISO 3166 code validation
Self-published format
 Resources
RFC 8805 - A Format for Self-Published IP Geolocation Feeds
https://www.rfc-editor.org/rfc/rfc8805.html
ISO 3166 Country Codes
https://www.iso.org/iso-3166-country-codes.html
 License
MIT License - see the LICENSE file for details.