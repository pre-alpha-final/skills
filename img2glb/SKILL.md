---
name: img2glb
description: "Create or refine a best-effort textured GLB model from reference images, including a small set of photos, with an interactive 3D preview for visual inspection and user review. Use for image-to-3D asset requests."
---

# img2glb

Turn the supplied images into a convincing, usable 3D asset with an interactive preview. Choose the modeling method to suit the object, evidence, and intended use. Visual correspondence matters alongside a valid export.

## Understand the references

- Inspect the available images before choosing geometry. Respect view labels, new close-ups, and user corrections. Preserve distinctive artwork, lettering, asymmetry, wear, and material character where supported.
- Map references to modeled regions. Compare silhouette, visible height/width, depth, feature placement, projection above the surrounding surface, and occlusion. Use comparable views and account for camera angle, roll, perspective, lighting, and fur overlap before turning pixel ratios into dimensions.
- Measure the visible feature against its visible counterpart. Hidden stuffing, an occluded chin, or a mesh's complete bounds may describe something different from the photographed outline.
- Preserve readable source files early and make derived textures separately. Verify paths before promising local reference links or preservation checks. An attachment can still provide visual evidence when its original path is unavailable; record that limitation and continue if the evidence is sufficient.
- Work with the available views. Ask for missing information only when it would materially improve the result, while continuing independent work. Keep unmeasured scale and inferred surfaces explicitly approximate.

## Build shape before surface detail

- Choose an appropriate approach: reference modeling, procedural construction, reconstruction, an available image-to-3D service, or a combination. There is no mandatory stack, topology, polygon count, or atlas layout.
- Check front and profile proportions early, then inspect a three-quarter view. A convincing frontal outline can conceal a flattened head or thin torso. Establish supported depth and attachment positions before spending heavily on surface detail.
- Represent volume that affects silhouette, parallax, shadows, or feature occlusion in geometry supported by the delivered format. Painted fluff cannot replace a furry outline or a plush rim that partly covers an eye. Verify these forms without textures.
- Project photographs onto suitable geometry and correct broad projection or exposure differences where useful. If eyes, noses, or other photographed features have separate geometry, remove their duplicate footprints from derived surface textures. Preserve the original images and meaningful markings.
- For plush, furry, or expressive characters, read [Soft surfaces and facial likeness](references/soft-surfaces-and-faces.md). It covers coat volume, recessed eyes, gaze, appendages, and profile corrections; it is conditional guidance, not a template for every object.
- Match geometry and texture cost to the intended use. Check file size and interactive performance. Choose a suitable representation or density rather than silently losing the volume the user requested; disclose substantial delivery costs or limitations.
- Embed geometry, materials, and textures in the GLB by default. Retain editable sources or settings and practical rebuild instructions.

## Refine without losing approved work

- Before a revision, identify the visual mismatch and the features the user has accepted. Treat a correction as a focused change. Preserve approved proportions and unrelated details unless the new evidence requires a coherent adjustment.
- Retain a practical baseline: settings, source, representative captures, and useful part measurements or hashes. Duplicate large binaries only when needed for recovery. Keep pending issues and accepted constraints understandable across revisions.
- Parameterize independently meaningful features, such as an attachment's base, tip, thickness, and direction, or an eye's mount, pupil, and surrounding aperture. A small tip correction should not require rescaling the whole feature.
- Keep procedural edits local. A fixed seed alone does not preserve geometry if filtering changes the number or order of random draws. Reuse samples, isolate random streams by part, or deform existing geometry so an eye edit does not regrow the entire coat or change unrelated textures.
- Move stuffing, coat, and attached parts coherently when changing volume. Update normals and tangents after deformation and check for folds, inverted faces, detached features, or exposed mounting surfaces.
- Rebuild the asset and refresh its preview together. Explain the observed cause and resulting change briefly; avoid replacing visual judgment with precise-looking statistics from uncertain photographs.

## Preview the delivered artifact

- Load the actual delivered GLB. Support orbit, zoom, pan, and reset/framing; fit the camera to its bounds and handle its real materials and parts.
- Provide useful comparison views and relevant close-ups, plus an untextured mode. A coat visibility switch can help inspect underlying sockets or stuffing when those are separate meshes. Do not impose a fixed six-face layout.
- Use clear, consistent lighting. Compare shape, material response, and reflections separately: a large environment highlight, a bright rim, or an exposed mount can change perceived shape or expression.
- Make view presets repeatable. Clear pending camera-control inertia before applying a preset and stop turntable motion for comparisons. Wait for model/textures and a settled view; finish saving a capture before advancing the camera or surface mode.
- Refresh the loaded asset after each build. Inspect representative angles, profile thickness, close-up occlusion, texture placement, seams, and material appearance yourself. Confirm captures show the current export and archive or replace outdated ones. Loading successfully is not visual verification.
- Keep the interface focused on inspection and make the GLB easy to download.

## Verify and deliver

- Validate the exported GLB, using the official glTF Validator when available, and check resource portability. Check finite attributes, normals, winding, and topology as relevant. Require closure only for parts intended to be closed; cloth labels and other deliberately open surfaces need different checks.
- Use meaningful checks for the requested change and approved invariants. Geometry hashes can prove exact preservation; bounds and ratios can track intended shape changes. A screenshot measurement depends on framing, lighting, and occlusion. Investigate a disagreement before changing geometry or relaxing a check, and do not claim more precision than the evidence supports.
- Keep reports and screenshots tied to the final artifact; a file hash is useful when revisions could be confused. Numerical validity does not establish likeness, expression, or visual quality.
- Deliver links to the GLB and interactive preview, a representative current screenshot, relevant source/rebuild information, and concise notes about significant limitations. State what was actually verified and make the result available for further visual feedback.
