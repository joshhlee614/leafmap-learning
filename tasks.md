

📦 Setup & Environment Tasks

✅ Task 1: Check if leafmap is installed
	•	Start: Assume leafmap may or may not be installed.
	•	End: Confirm installation using pip show leafmap or conda list.

⸻

✅ Task 2: Import the leafmap module
	•	Start: Start with an empty Python file.
	•	End: Successfully run import leafmap without errors.

⸻

✅ Task 3: Create your first leafmap.Map() object
	•	Start: Import leafmap.
	•	End: Create a map object using m = leafmap.Map() and confirm it exists.

⸻

✅ Task 4: Display the empty map
	•	Start: Map object created.
	•	End: Render the map in a Jupyter notebook or Streamlit app.

⸻

🗺️ Map Construction Basics

✅ Task 5: Center the map on a coordinate
	•	Start: Have a basic map object m.
	•	End: Center the map using leafmap.Map(center=[latitude, longitude]).

⸻

✅ Task 6: Set the initial zoom level
	•	Start: Map is centered.
	•	End: Set zoom= in the Map() constructor and observe the zoom.

⸻

✅ Task 7: Add a basemap layer
	•	Start: Have a visible map.
	•	End: Use m.add_basemap('HYBRID') or another available option.

⸻

✅ Task 8: List all available basemaps
	•	Start: Leafmap is imported.
	•	End: List them with leafmap.basemaps.keys().

⸻

📍 Adding Basic Layers

✅ Task 9: Add a single marker
	•	Start: Know a location (e.g. UT Austin).
	•	End: Add it with m.add_marker(location=[lat, lon], popup="Label").

⸻

✅ Task 10: Add multiple markers from a Python list
	•	Start: Have a list of coordinates.
	•	End: Loop through and call add_marker() for each.

⸻

📂 Working with External Data

✅ Task 11: Load points from a CSV file
	•	Start: Have a CSV with columns lat, lon, label.
	•	End: Use m.add_points_from_xy() or loop and add manually.

⸻

✅ Task 12: Load a GeoJSON file
	•	Start: Have a local or URL GeoJSON file.
	•	End: Use m.add_geojson("path_or_url.geojson").

⸻

✅ Task 13: Load a shapefile
	•	Start: Have a .shp, .shx, .dbf set.
	•	End: Use m.add_shapefile("folder_path").

⸻

✅ Task 14: Style a vector layer
	•	Start: Add a GeoJSON or shapefile.
	•	End: Set style={'color': 'red', 'fillOpacity': 0.5} in the add call.

⸻

🌈 Working with Raster Data

✅ Task 15: Load and display a GeoTIFF
	•	Start: Have a local raster file.
	•	End: Use m.add_raster("your_file.tif").

⸻

✅ Task 16: Add remote raster tiles
	•	Start: Find tile server URL.
	•	End: Use m.add_tile_layer(url=..., name="Layer Name").

⸻

🧭 Controls and Tools

✅ Task 17: Add a layer control widget
	•	Start: Add multiple layers.
	•	End: Call m.add_layer_control() to toggle visibility.

⸻

✅ Task 18: Add a time slider
	•	Start: Have temporal data.
	•	End: Use m.add_time_slider() and verify slider appears.

⸻

🧪 Interactivity and Analysis

✅ Task 19: Add a drawing tool
	•	Start: Basic map ready.
	•	End: Use m.add_draw_control() to interactively draw.

⸻

✅ Task 20: Capture geometry from drawn shapes
	•	Start: Drawing control enabled.
	•	End: Print or save the geometry from drawn objects.

⸻

🌐 Exporting and Sharing

✅ Task 21: Export map as HTML
	•	Start: Map is built.
	•	End: Use m.to_html("output.html") and open in browser.

⸻

✅ Task 22: Embed map in Streamlit or Panel
	•	Start: Build or scaffold a web app.
	•	End: Display using st.components.v1.html() or similar.

⸻

🧠 Wrap-Up: Mini Project

✅ Task 23: Plot Texas colleges from CSV
	•	Start: Have a CSV of Texas colleges with coordinates.
	•	End: Load the data and display each with a popup label.