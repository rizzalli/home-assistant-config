# Home Assistant Config

Personal configuration for Home Assistant, including YAML-based automations,
scripts, themes, and the Adaptive Lighting custom integration.

## Adaptive Lighting Profiles

Adaptive Lighting is defined in `adaptive_lighting.yaml`. Recent changes:

- Use only individual light entities per profile to prevent duplicate service
  calls and flickering.
- Enable `detect_non_ha_changes` everywhere so manual overrides are respected
  when `take_over_control` is on.
- Split pantry and laundry fixtures into distinct profiles so they no longer
  fight each other for control.

Reload or restart Adaptive Lighting after modifying the YAML to apply updates.
