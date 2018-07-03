- Added new feature, [yAxis.angle](https://api.highcharts.com/highcharts/yAxis.angle), allowing positioning the axis line and labels in polar chart Y axes. This makes it practical to use multiple axes in polar charts.
- Added option, [xAxis.nameToX](https://api.highcharts.com/highcharts/xAxis.nameToX), allowing points to have the same name but different axis positions on an axis of type ``category``.
## Bug fixes 
- Fixed #1011, ``ignoreHiddenSeries`` with ordinal axis caused artefacts on a chart.
- Fixed #1041, gaps in the area fill of stacked areasplines.
- Fixed #3169, error on drilldown from a null point.
- Fixed #3341, exceeded stack size on mutually linked series.
- Fixed #3571, NaN in the beginning of data broke series.
- Fixed #4778, wrong rendering waterfall series, when yAxis.max was set.
- Fixed #5186, gaps in the fill of areasplinerange.
- Fixed #5383, mouse position detection with ``pointPlacement``.
- Fixed #5528, a regression causing polar arearanges to fail.
- Fixed #5533, ``stickyTracking`` when set to false caused highlighting wrong point.
- Fixed #5552, linejoins in boost module lines.
- Fixed #5556, JS error on polygon with empty data.
- Fixed #5563, JS error in treemap with zero values.
- Fixed #5568, ``pointIntervalUnit`` broke when using more data points than ``turboThreshold``.
- Fixed #5569, generic options set on the ``yAxis`` affected the ``colorAxis``.
- Fixed #5570 and #5590, regression causing blank export on Batik based export servers.
- Fixed #5572, pie slices were not hidden in 3D pie charts on legend click.
- Fixed #5595, HTML tooltip did not hide on point mouse out via the tooltip.
- Fixed #5605, error on async onload of destroyed chart.
- Fixed #5618, updating master series caused wrong visibility on linked series.
- Fixed #5619, the Series remove event was fired when updating a series.
- Fixed #5620, text was mispositioned when loading a chart in a hidden iframe in certain browsers.
- Fixed #5622, click event for line series point was not called when column was rendered below.
- Fixed #5631, zeroes in logarithmic chart made the whole graph crash.
- Fixed #5632, gaps were broken in arearange and areasplinerange.
- Fixed #5646, waterfall did not work correctly with logarithmic axis.
- Fixed #5647, xrange points disappeared if x was outside plot but x2 inside.
- Fixed #5647, xrange points disappeared when x was outside visible range.
- Fixed #5655, ``animation: true`` on a series config caused animation to jump from the middle.
- Fixed #5658, error on updating series from its own ``mouseOver`` event.
- Fixed #5662, ``setExtremes`` on polar chart caused padded max value.
- Fixed #5665, ``addPoint`` animation parameter was not used.
- Fixed #5679, handle isArray for ES6 iterator.
- Fixed #5681, JS error on adding custom group to points.
- Fixed #5689, text had soft line wraps when ``white-space: nowrap`` was used in combination with text-overflow: ellipsis.
- Fixed issue #4133, error bar data labels positions failing on redraw.
- Fixed issue #5205, color axis changed colors when legend was disabled.
- Fixed issue #5567, wrong clipping of offline exported SVG in IE11/Edge.
- Fixed wrong handling of ``minRange`` on logarithmic axis, related to #1227.