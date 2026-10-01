# CIELAB measurement code

All five Python scripts support the project's CIELAB measurement workflow. The first two prepare video frames for measurement, `lab_image_analysis.py` calculates the image-level CIELAB values, and the final two scripts combine and compare those values across clips and narrative stages.

| Script | Role in the workflow |
| --- | --- |
| `avg_shot_length.py` | Detects shot boundaries in a designated video and reports its duration, shot count, and average shot length. This helps assess the video sampling plan; it does not calculate CIELAB values. |
| `capture_screenshots.py` | Extracts still frames from MP4 clips at a chosen interval (4.75 seconds by default) and saves timestamped images in a `screenshots` folder. These images are the inputs for CIELAB measurement. |
| `lab_image_analysis.py` | Reads PNG screenshots and measures CIELAB lightness (`L`), color channels (`a` and `b`), chroma, high-chroma area, and lightness contrast. It writes image-level results plus an overall average to `lab_summary.csv`, adds descriptive visual-feeling labels, and saves two metric plots. |
| `visual_trend_across_clips.py` | Collects clip-level LAB summary CSVs, creates a combined CSV with an image-count-weighted all-clips average, and plots CIELAB trends across selected clips. It also saves a table image of the clip-level visual descriptions. |
| `compare_lab_sets.py` | Compares combined LAB summaries for the Setup and three narrative acts. It writes `lab_set_average_summary.csv`, including an image-count-weighted `all sets` row, and plots the stage-level CIELAB metrics. |

Some scripts contain anonymized default paths beginning `/Users/xxxx/xxxx`. Provide the appropriate local paths through their command-line options, where available, or update the defaults before running them.
