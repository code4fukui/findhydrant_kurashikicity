# findhydrant_kurashikicity

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A web application to search for fire hydrants and other firefighting water sources in Kurashiki City, Okayama Prefecture, Japan, using open data.

## Demo

**https://github.com/code4fukui/findhydrant_kurashikicity


![Screenshot of the findhydrant_kurashikicity application showing a map of Kurashiki with icons for hydrants. A popup is open on one hydrant, displaying its details.](ss.jpg)


## Features

-   **Map-based Visualization**: Displays the locations of fire hydrants and water cisterns on an interactive map.
-   **Geolocation**: Automatically detects the user's current location to center the map and find nearby water sources.
-   **Nearest Search**: Instantly calculates and highlights the closest fire hydrant to your location.
-   **Detailed Information**: Click on any icon to view details such as the type of water source, address, and pipe diameter.
-   **Dynamic Icons**: Uses distinct icons to differentiate between hydrants, cisterns, and other water sources.
-   **Multi-language Support**: The interface automatically adapts to your browser's language settings (Japanese, English, and more).

## Usage

1.  Open the [demo application](https://code4fukui.github.io/findhydrant_kurashikicity/).
2.  Allow the browser to access your location when prompted.
3.  The map will display nearby fire hydrants.
4.  Click the "find nearest" button to navigate to the closest hydrant.
5.  Click any hydrant icon on the map to see its details.

## Data Source

This application uses a bundled CSV file derived from the "消防水利（消火栓、防火水そう等）" (Firefighting Water Sources) dataset provided by Kurashiki City.

-   **Data Origin**: [Okayama Open Data Portal](https://www.okayama-opendata.jp/resources/14754)
-   **Local Data File**: [`332020_fire_hydrant_202404_standard.csv`](332020_fire_hydrant_202404_standard.csv)

The data is processed and loaded directly from the local file within the application; no live API calls are made for hydrant data.

## Built With

-   [Leaflet](https://leafletjs.com/) with [GSI map tiles](https://maps.gsi.go.jp/) via `LeafletGSI.js`
-   [Geo3x3](https://geo3x3.com/) for geographic coordinate encoding
-   Vanilla JavaScript (ES Modules)

## Author

-   [taisukef](http://fukuno.jig.jp/)

## License

This project is available under the MIT License - see the [LICENSE](LICENSE) file for details.