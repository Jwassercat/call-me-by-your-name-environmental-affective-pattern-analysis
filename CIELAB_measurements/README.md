# CIELAB measurements for 24 clips and whole film CIELAB trend

This folder contains the `lab_summary.csv` files from `call_me_by_your_name/clips/clip1` through `clip24`. Each file is named `lab_summary_clipN.csv`, where `N` is the clip ID. The original CSVs remain in their clip folders.

Each CSV has one row per analyzed screenshot or video frame. It records the image filename and source path, image dimensions, CIELAB lightness (`L`) and color channels (`a`, `b`), chroma and contrast measures, and a brief `visual_feeling` description. The `visual_feeling` description field was not consulted in the research. The `source_path` values refer to the original local files.

This folder also contains `lab_set_average_summary.csv` file from the comparison of all narrative stages. The figure `lab_set_average_trends.png` visualizes the development of all visual parameters across the four narrative stages throughout the film.