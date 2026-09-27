# pyqt-temperature-plotter

A small PyQt5 desktop app that plots daily temperatures from a CSV file as a line or bar chart, drawn with Matplotlib inside the window.

Pick a start date and an end date, choose **Line Graph** or **Bar Graph**, and press **Plot**.

## What's in here

| File | What it does |
|---|---|
| `app.py` | The app. A `TemperatureGraphApp` window with two date pickers, a graph-type dropdown, a Plot button and a Matplotlib canvas. |
| `source_file_generator.py` | Writes `temperature_data.csv` with one random reading between -10 and 40 for every day of 2023. |
| `temperature_data.csv` | Sample data made by the generator, with `Date` and `Temperature` columns. |

## Run it

```
git clone https://github.com/Muntaha-Islam0019/pyqt-temperature-plotter.git
cd pyqt-temperature-plotter
pip install PyQt5 matplotlib
python app.py
```

The date pickers open on the last 7 days, but the sample data covers 2023, so set both dates inside 2023 before pressing Plot.

To plot your own data, replace `temperature_data.csv` with a file that has a `Date` column (YYYY-MM-DD) and a `Temperature` column. To get a fresh random year instead, run `python source_file_generator.py`.

## License

MIT. See [LICENSE](LICENSE).
