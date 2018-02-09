# Maine Lyme Disease Portal Data

To replicate the source data set:

- Go [here](https://gateway.maine.gov/cognos/cgi-bin/cognosisapi.dll?b_action=cognosViewer&ui.action=run&ui.object=%2fcontent%2ffolder%5b%40name%3d%27CDC%20EOHP%20EPHT%20AVR%27%5d%2freportView%5b%40name%3d%27Maine%20Environmental%20Public%20Health%20Tracking%20%28EPHT%29%20Network%20-%20Public%20Data%20Portal%27%5d&cv.header=false&cv.toolbar=false)
- Find the lyme rectangle and hit the data link
- Tables tab
- Use selector on right
- When "happy" => use the **PDF** link at bottom right
- Sceen comes up
- Choose XML view
- Copy/paste XML

I chose:

- Incidence
- Counties
- Rate
- Selected 2001 - 2016
- Sex: Both
- Ages: all years
- All counties

I did ^^ b/c at some level with more detail, some data elements aren't populated.

Source: `maine-lyme-2001-2016.xml`

Tidy: `maine-lyme-2001-2016.csv`

I'm going to try to use `splashr` to do ^^ in a reproducible way

