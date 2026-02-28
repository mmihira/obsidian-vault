---
task: pixel-art-generation
template: "[[Pixel Art Generation/Prompt template.md]]"
status: generated
date: 2026-02-22
---

# Pixel Art Generation Task

> Fill in the two sections below, then ask Claudian to **generate the prompt**.
> Claudian will merge your inputs with the [[Pixel Art Generation/Prompt template.md]] and output a ready-to-use generation prompt.

---

## 🖼️ Visual Reference

![[Screenshot 2026-02-22 at 4.35.59 pm.png]]
---

## ✏️ Text Prompt

The tower in the middle is not big enough nor does it match the overall color scheme



---

## ⚙️ Overrides *(optional)*

<!-- Override any defaults from the Prompt template. Leave blank to use template defaults.
     Fields you can override:
       - target_style         → e.g. "8-bit", "32-bit", "CGA", "Game Boy"
       - output_resolution    → e.g. "16x16", "32x32", "64x64"
       - palette_quantization → e.g. "4_colors_max", "16_colors_max"
       - dithering_algorithm  → e.g. "none", "Floyd-Steinberg", "Bayer_Ordered_Matrix"
-->

| Field | Value |
|---|---|
| target_style | |
| output_resolution | |
| palette_quantization | |
| dithering_algorithm | |

---

## 📋 Generated Prompt

<!-- Claudian will write the final prompt here after you ask. Do not edit manually. -->

```json
{
  "task_definition": {
    "type": "pixel_art_generation",
    "target_style": "16-bit_retro_console",
    "output_resolution": "native_grid_alignment",
    "subject": "central_tower_shrine_structure",
    "action": "redraw_rescale_recolor"
  },
  "technical_constraints": {
    "anti_aliasing": "DISABLED",
    "grid_snap": "STRICT_8x8_VIRTUAL_PIXELS",
    "dithering_algorithm": "Floyd-Steinberg",
    "noise_pattern": "Bayer_Ordered_Matrix",
    "palette_quantization": "32_colors_max"
  },
  "visual_reference": {
    "structure": "adhere_to_input_grid_frequency",
    "texture": "interpret_noise_as_pixel_detail",
    "source_image": "Screenshot 2026-02-22 at 4.35.59 pm.png",
    "perspective": "top_down_south_facing_lean"
  },
  "edit_instructions": {
    "scale": {
      "problem": "tower_is_approximately_player_height",
      "target": "2.5x_to_3x_player_height",
      "tile_estimate": "3_to_4_tiles_tall",
      "intent": "landmark_not_prop"
    },
    "color": {
      "problem": "cold_navy_blue_does_not_match_scene_palette",
      "eliminate": "all_cold_navy_and_slate_blue_tones",
      "target_palette": {
        "grass_and_canopy": "warm_sage_green_approx_#6a9e3c",
        "grass_accents": "muted_olive_highlights",
        "stonework": "desaturated_gray_with_warm_undertones",
        "earthy_detail": "warm_brown_approx_#8b5a2b"
      },
      "palette_source": "match_existing_scene_tile_colors"
    },
    "form": {
      "silhouette": "cylindrical_stacked_stone_with_lantern_crown",
      "added_detail": ["moss_patches_on_lower_stones", "vine_pixel_detail"],
      "intent": "integrate_structure_with_grass_environment"
    }
  },
  "output": {
    "background": "transparent",
    "format": "isolated_asset",
    "grid_alignment": "tile_edges_on_8x8_scene_grid",
    "seams": "none"
  }
}
```

---

*To generate: fill in the sections above, then say **"generate the prompt"**.*
