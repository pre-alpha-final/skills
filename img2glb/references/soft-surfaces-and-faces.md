# Soft surfaces and facial likeness

Use this guidance for plush, furry, padded, or expressive characters. Apply the observations supported by the references. There is no universal head ratio, pupil ratio, eye direction, or strand count.

## Real coat volume

- Separate the stuffed silhouette from the pile envelope. Undercoat fills gaps; longer tufts establish softness, direction, and irregular edges. Regional length, thickness, density, clumping, and grooming matter more than a single dense noise layer.
- Model pile that contributes to depth or occludes features. Curved solid fibers or clumps can work when portable volumetric geometry is needed; other representations can suit different budgets. Verify that the chosen hair, transparency, or instancing method survives GLB export and the intended viewer.
- Inspect the coat in profile and clay mode. Look for an underlying bare-looking shape, sparse gaps, flat cards, unnaturally regular spikes, or the same fiber scale everywhere. Extra polygons alone do not create convincing softness.
- Preserve the supporting stuffing and neighboring coat during grooming changes. Reusing the existing yarn layout can make a local correction more predictable than regenerating the whole surface.

## Eyes, gaze, and expression

Compare these together in a frontal close-up and a three-quarter view:

- Outer eye size relative to the visible face, eye spacing, eye-line height, and placement relative to the nose or beak.
- Physical eye shape versus its projected outline. A round eye can appear oval from the side or beneath fur; forcing every visible outline into a complete circle can lose likeness.
- Pupil or black-center size relative to the actual eye, including parts hidden by pile. A photographed visible bounding box is not necessarily the full iris diameter.
- Apparent pupil direction, lens depth, exposed glitter or colored rim, surface reflections, and surrounding fur overlap.

Treat the mount, black center, and furry aperture as related but separately adjustable forms. A mount may follow the curved head while an offset domed lens makes its center appear to look outward. Check the resulting gaze from multiple views; choose alignment from the reference rather than always centering pupils in screen space or always shifting them inward.

A startled or fixed stare can come from fully exposed bright rings, excessive lens bulge, mismatched pupil proportions, divergent alignment, or oversized catchlights. Diagnose which cues differ before editing. A wider black center, shallower lens, adjusted alignment, darker rim, or softer reflections may help a particular reference, but none is a universal correction.

Plush eyes often sit inside padded sockets. Model and groom the upper and inner pile so it can partly cover the rim where the photo shows this. Uniformly combing every strand away from the lens exposes a clean annulus and can change the expression. Prefer physical fur overlap or supported surface volume over painting a shadow around an otherwise exposed eye.

Inspect eye seating from the side. Avoid a floating iris plate, visible backing, detached collar, or lens far above the surrounding pile. Preserve a clear pupil while letting stuffing and coat frame it. Keep natural irregularity supported by the references; perfect bilateral exposure is not always a likeness improvement.

Use a consistent lighting setup to distinguish geometry from material response. Large environment panels can create broad reflections that resemble a fixed artificial gaze. Adjust lens curvature, roughness, clearcoat, or comparison lighting deliberately, keeping the exported material representative of the result. Do not bake photographed catchlights into a surface and then unintentionally add a second set through glossy geometry.

## Small projecting features

Judge a beak, nose, horn, or similar feature by its visible projection above the surrounding coat, not only its length from the stuffing center. A buried thick base can support a very short visible tip.

Keep base attachment, thickness, axis, taper, and distal point independently controllable. Follow the reference's direction and profile. Shortening the whole mesh can erase the stuffed base; rounding everything can remove a defining point. Refine the distal region when that is what the user requests, then inspect both frontal shape and side projection through the actual fur.

## Fuller profiles without changing the face

Use a side reference to judge head depth and torso depth separately, with their silhouettes compared at similar scale and angle. Include the pile envelope and distinguish the body from wings, tail, and labels. A deep head and a shallow torso, or the reverse, may both be plausible depending on the subject.

When the user has approved the front, consider adding volume behind the face while preserving frontal feature coordinates. Move stuffing and coat together, and carry wings, tail, or other attachments with their supporting surface. Preserve eye and nose/beak shape unless their seating actually needs adjustment. Recompute transformed normals and tangents, and inspect the front again after the profile change.

Keep the correction coherent rather than applying a uniform whole-model scale. A depth change should not automatically thicken the eyes, lengthen the beak, enlarge the feet, or expose attachment seams.

When checking a local grooming correction, distinguish changed fiber tips from the supporting form. Upper eye yarn can move forward or down while the stuffing and rear profile stay fixed. Compare the relevant close-up, an oblique or profile view, and untextured geometry; use regression measurements that reflect those intended changes.
