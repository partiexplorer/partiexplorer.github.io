---
comments: false
---

# La route 138

Mon exploration de la route 138 vers Kegaska ma fait parcourir 
2712.7km sur 6 jours.

## La Prairie à Tadoussac

2022-10-23

468.6km

<div id="mapid" style="height: 400px;width: 600px"></div>

<script type="text/javascript">
  document.addEventListener("DOMContentLoaded", function() {

    // Create a new map with a fullscreen button:
    var map = new L.Map('mapid', {
        fullscreenControl: {
            pseudoFullscreen: true // if true, fullscreen to page width and height
        }
    });

    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
        maxZoom: 12,
        attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a>'
    }).addTo(map);

    L.control.scale({imperial: false}).addTo(map);

    var gpx = '/assets/gpx/2022-10-23_LaPrairie-Tadoussac.gpx'; // URL to your GPX file or the GPX itself
    new L.GPX(gpx, {
      async: true,
      marker_options: {
        startIconUrl: '',
        endIconUrl: '',
        shadowUrl: ''
      }
    }).on('loaded', function(e) {
      map.fitBounds(e.target.getBounds());
      // e.target.get_distance()
    }).addTo(map);

  })
</script>

## Tadoussac - Franquelin

2022-10-24

272.6km

![track](../assets/images/route138/track_2022-10-24.png){ width="480" }

## Franquelin - Pointe-à-Mingan

2022-10-25

391.6km

![track](../assets/images/route138/track_2022-10-25.png){ width="480" }

## Pointe-à-Mingan - Kegaska

2022-10-26

236.7km

![track](../assets/images/route138/track_2022-10-26a.png){ width="480" }

## Kegaska - Pointe-à-Mingan

2022-10-26

236.6km

![track](../assets/images/route138/track_2022-10-26b.png){ width="480" }

## Pointe-à-Mingan - Franquelin

2022-10-27

388.8km

![track](../assets/images/route138/track_2022-10-27.png){ width="480" }

## Franquelin - La Prairie

2022-10-28

717.8km

![track](../assets/images/route138/track_2022-10-28.png){ width="480" }
