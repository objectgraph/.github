<div align="center">

# ObjectGraph

### Apps for Apple platforms, since day one of the App Store.

ObjectGraph LLC, New York. Founded 2004. **iRetroPhone** shipped on July 10, 2008, the day
the App Store opened, and about 145 apps have followed. Today the work is map and GPS tools,
a seismograph you can hold, and — under the VooV name — an AI workspace.

[**objectgraph.com**](https://www.objectgraph.com) &nbsp;·&nbsp; [App Store](https://apps.apple.com/us/developer/objectgraph-llc/id284700705) &nbsp;·&nbsp; [Blog](https://www.objectgraph.com/blog) &nbsp;·&nbsp; [VooV / Catalyst →](https://github.com/voovai)

</div>

---

## Products

| Product | What it is | Repositories |
| --- | --- | --- |
| [**iRetroPhone**](https://iretrophone.com) · [App Store](https://apps.apple.com/us/app/id284700702) | A rotary dial phone for iPhone and iPad. On the store since opening day 2008; version 3 is a SwiftUI rewrite of the original. | [`iRetroPhone`](https://github.com/objectgraph/iRetroPhone) app · [`iretrowww`](https://github.com/objectgraph/iretrowww) site · [`iretrophone-wrapper`](https://github.com/objectgraph/iretrophone-wrapper) specs |
| [**Seismograph / iSeismometer**](https://seismograph.com) · [App Store](https://apps.apple.com/us/app/id304190739) | Your phone as a three-axis seismograph and your Mac as the receiver for a home seismic network. iPhone, iPad and Mac. | [`ISeismometerSwift`](https://github.com/objectgraph/ISeismometerSwift) app · [`seismowww`](https://github.com/objectgraph/seismowww) site · [`seismograph`](https://github.com/objectgraph/seismograph) specs |
| **Geo Measure** · [iOS](https://apps.apple.com/us/app/id451326903) · [Mac](https://apps.apple.com/us/app/id735322124) · [Web](https://www.geosq.com/geomeasure) | Area and distance on a map: how big is that farm, how far to the station. | [`GeoMeasureMulti`](https://github.com/objectgraph/GeoMeasureMulti) iOS / iPadOS / macOS · [`GeoMeasureMac`](https://github.com/objectgraph/GeoMeasureMac) · [`geomeasure_osm`](https://github.com/objectgraph/geomeasure_osm) OpenStreetMap web (public) |
| **Geo Elevation** · [iOS](https://apps.apple.com/us/app/id509924746) · [Mac](https://apps.apple.com/us/app/id1096825035) · [Web](https://www.geosq.com/geoelevation) | The elevation profile of any path or point on a map. | [`GeoElevation`](https://github.com/objectgraph/GeoElevation) · [`GeoElevationMac`](https://github.com/objectgraph/GeoElevationMac) |
| **Geo Tracker** · [App Store](https://apps.apple.com/us/app/id627038315) | Record routes with GPS and keep them as GPX. Everything stays on the device. | [`GeoTracker`](https://github.com/objectgraph/GeoTracker) |
| **Seismica** · [App Store](https://apps.apple.com/us/app/id6746057677) | A live earthquake map. | [`Seismica`](https://github.com/objectgraph/Seismica) |

Also on the App Store: [GPX Explore](https://apps.apple.com/us/app/id6745435014), a GPX track
viewer for iOS and Mac, and [WorkoutGPX](https://apps.apple.com/us/app/id6743941036), which turns
Apple Health workouts into GPX files. The AI work — **Catalyst**, every AI in one workspace — lives
in the [voovai](https://github.com/voovai) organization.

---

## Where things live

| Repository | What it is |
| --- | --- |
| [`apple`](https://github.com/objectgraph/apple) | The Apple developer account as code: App Store Connect CLI, the push-notification recipe, the app inventory, and one wrapper folder per product |
| [`ogwww`](https://github.com/objectgraph/ogwww) | [objectgraph.com](https://www.objectgraph.com) and the blog — Astro on Cloudflare |
| [`geosq`](https://github.com/objectgraph/geosq) | [geosq.com](https://www.geosq.com) — Geo Measure and Geo Elevation on the web |
| [`httplabs`](https://github.com/objectgraph/httplabs) | [httplabs.com](https://httplabs.com) (public) |
| [`samegame`](https://github.com/objectgraph/samegame) · [`SameGameBlazor`](https://github.com/objectgraph/SameGameBlazor) | SameGame, the puzzle, in JavaScript and in Blazor (public) |
| [`electron-pdf-window`](https://github.com/objectgraph/electron-pdf-window) | View PDF files in Electron browser windows (public) |

---

## How a product is laid out

Every current product is three repositories under one wrapper folder:

- **The wrapper** (`seismograph`, `iretrophone-wrapper`) holds the shared specs — file formats,
  wire protocols, dial geometry — that the app and the site both have to honour.
- **The app** is a single Xcode project, SwiftUI, built and archived by Xcode Cloud on push.
- **The site** is static (Astro or plain HTML) and deploys to Cloudflare on push.

The app is the source of truth for behaviour; the site describes it and must stay true to it.

---

<div align="center">
<sub>ObjectGraph LLC · New York · <a href="https://www.objectgraph.com">objectgraph.com</a></sub>
</div>
