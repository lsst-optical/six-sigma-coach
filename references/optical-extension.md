# Optical Engineering Extension

Load this reference only for optical, imaging, lens, optomechanical, optoelectronic, or CODE V problems.

## Operationally defining optical Y

An optical metric name is not yet a CTQ. Define conditions that change meaning:

- product/configuration and serial or build state;
- focal length, object distance, conjugate, focus method, aperture/F-number, zoom/focus direction;
- field/relative image height, azimuth, wavelength or spectrum, polarization when relevant;
- spatial frequency and sagittal/tangential orientation for MTF;
- temperature, humidity, pressure, pose, gravity direction, vibration state, warm-up and time;
- fixture, datum, remount/refocus rule, algorithm/software version, sampling and pass rule;
- center, edge, minimum-of-fields, average, percentile, yield, or another aggregation.

Keep customer experience and engineering metrics traceable. Examples:

- “long-end edge looks soft” → MTF at specified focal length, aperture, field, spatial frequency, orientation, focus/remount protocol, and minimum/percentile rule;
- “AF is slow” → step size, direction, illumination/contrast, temperature, load, response/settling definition, overshoot and success rate;
- “zoom feels rough” → torque curve versus position, direction, speed, pose, temperature, aging and hysteresis;
- “image shifts” → coordinate system, focus/zoom path, pose, thermal state, reference, repeatability and drift.

## Optical measurement-system risks

MSA should represent the entire measurement chain, not only gauge resolution:

- source stability, spectrum, detector linearity/noise and calibration;
- target, collimator, interferometer, MTF bench or camera alignment;
- fixture datum, clamp force, gravity pose, remount and refocus;
- operator choices, autofocus/search algorithm and stopping rule;
- image processing, ROI, threshold, software/version and data export;
- environmental stability and sample change during measurement.

For destructive or non-repeatable tests, do not force a crossed GRR. Consider nested or expanded designs. Separate repeatability, reproducibility, bias, linearity, stability, resolution and sample representativeness.

## System and interface thinking

Trace each CTQ through functions and interfaces:

- optical prescription, glass, surface figure, centration, tilt, spacing and coatings;
- barrel/datums, guide/cam geometry, fit, torque, preload, adhesive, cure and assembly stress;
- actuator, sensor, current, thermal load, power, electronics and EMC;
- firmware/control law, calibration, compensation, diagnostic and fail-safe behavior;
- manufacturing capability, fixture, EOL test, repair and field environment.

Subsystem compliance does not prove system compliance. Use N²/interface matrices, tolerance analysis, FMEA/FTA and DVP&R to expose couplings.

## Simulation and DOE boundary

- CODE V tolerance/sensitivity and Monte Carlo output is model evidence, not production capability by itself.
- Preserve correlation, non-normal manufacturing distributions, assembly adjustment strategy and truncation assumptions where material.
- Use physics and simulation to narrow factors and safe ranges; use designed experiments or representative builds to validate the real system.
- When optimizing image quality, include guardrails such as center/edge balance, distortion, relative illumination, CRA, package, mass, cost, focus/zoom behavior and manufacturability as applicable.

## Typical optical tool chain

`VOC → CTQ/QFD → system boundary/functional architecture → tolerance and interface analysis → SFMEA/DFX → MSA/DVP&R → DOE or robust optimization → pilot capability/SPC → control plan/SOP/lessons learned`

Choose only the steps needed for the decision.

