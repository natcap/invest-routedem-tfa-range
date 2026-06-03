# About
This plugin provides an alternative version of the core InVEST RouteDEM utility. This version replaces the standard "Threshold Flow Accumulation" input value with a "Threshold Flow Accumulation Range" input, which allows the model to compute outputs for a range of TFAs in a single run.

Threshold Flow Accumulation (TFA) is a stream delineation algorithm parameter that specifies the number of upstream pixels that must flow into a pixel before it is classified as a stream. Since Threshold Flow Accumulation is only relevant in cases where streams are calculated from the flow accumulation output, this plugin always calculates flow direction, flow accumulation, and streams. 

## Threshold Flow Accumulation Range
In this plugin, the "Threshold Flow Accumulation Range" input takes the form ``start_value:stop_value:step_value``, where:
- ``start_value``: An integer specifying at which value to start.
- ``stop_value``: An integer specifying at which value to stop (not inclusive).
- ``step_value``: An integer specifying the incrementation from the ``start_value`` up to the ``stop_value``.

The model inputs are otherwise identical to those of the [InVEST RouteDEM utility](https://storage.googleapis.com/releases.naturalcapitalproject.org/invest-userguide/latest/en/routedem.html).
