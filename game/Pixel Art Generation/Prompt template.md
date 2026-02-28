{
"task_definition": {
"type": "pixel_art_generation",
"target_style": "16-bit_retro_console",
"output_resolution": "native_grid_alignment"
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
"texture": "interpret_noise_as_pixel_detail"
}
}
