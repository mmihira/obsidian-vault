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
      "perspective": "SNES_RPG_top_down_like_Zelda_ALTTP_or_Secret_of_Mana_camera_directly_above_tilted_slightly_south_tower_shows_ONLY_fr
  ont_face_and_narrow_top_surface_ZERO_side_faces_visible_left_edge_and_right_edge_are_symmetrical_vertical_lines_THIS_IS_NOT_ISOMETRIC"
    },
    "edit_instructions": {
      "improve_tower": {
        "goal": "redesign_tower_as_level_1_attack_tower_in_power_network_while_preserving_scene_aesthetic",
        "context": "tower_is_a_level_1_attack_structure_that_receives_energy_from_a_power_network_and_fires_magic_projectiles",
        "material": {
          "primary": "sturdy_wooden_construction_thick_timber_beams_and_planks",
          "feel": "solid_and_functional_not_flimsy_or_makeshift",
          "texture": "visible_wood_grain_via_pixel_dithering_warm_browns_and_tans",
          "constraint": "no_brick_or_stone_this_is_wood_but_should_look_well_built"
        },
        "tower_shape": {
          "body": "wooden_tower_that_tapers_inward_toward_the_top",
          "top_surface": "flat_narrowed_platform_at_top_created_by_the_taper",
          "taper_style": "gradual_narrowing_of_planks_not_a_sudden_step",
          "constraint": "taper_creates_a_snug_cradle_or_seat_for_the_crystal_emitter_at_the_peak"
        },
        "emitter_crystal": {
          "location": "sitting_on_top_surface_of_tower_nestled_into_the_tapered_peak",
          "concept": "small_cyan_crystal_that_fires_magic_projectiles",
          "visual_cues": "glowing_cyan_gem_sitting_snugly_on_the_narrowed_top_platform",
          "size": "small_1x1_or_2x2_pixel_cluster",
          "constraint": "crystal_is_the_topmost_element_of_the_tower_no_post_or_bracket_needed_the_taper_holds_it"
        },
        "power_receiver_ring": {
          "location": "horizontal_band_across_front_face_near_top_of_tower",
          "concept": "glowing_cyan_energy_band_visible_as_a_horizontal_line_across_the_tower_front",
          "visual_cues": "thin_horizontal_cyan_pixel_line_spanning_the_width_of_the_front_face_with_slight_curve_visible_on_top_surface",
          "color": "same_cyan_as_emitter_crystal_to_show_they_are_connected",
          "width": "1_to_2_pixels_tall",
          "constraint": "render_from_three_quarter_top_down_perspective_only_front_and_top_visible_do_not_wrap_around_sides"
        },
        "size": {
          "target": "approximately_1.5x_player_character_height_max",
          "footprint": "compact_no_wider_than_1_tile",
          "constraint": "this_is_a_small_level_1_tower_not_a_siege_engine_keep_it_modest"
        },
        "perspective": {
          "view": "SNES_RPG_top_down_NOT_isometric",
          "camera": "directly_above_tilted_slightly_south",
          "visible_faces": "front_face_and_narrow_top_surface_ONLY",
          "left_and_right_edges": "must_be_symmetrical_vertical_lines_no_diagonal_edges",
          "forbidden": "ABSOLUTELY_NO_isometric_view_NO_diagonal_rotation_NO_side_faces_NO_3D_perspective_NO_vanishing_points",
          "examples": "think_Zelda_A_Link_to_the_Past_or_Secret_of_Mana_buildings",
          "reference": "tower_must_match_exact_same_perspective_as_bushes_walls_and_trees_already_in_the_scene",
          "test": "if_you_can_see_the_left_or_right_wall_of_the_tower_you_are_wrong_redo_it"
        },
        "shading": "improve_light_and_shadow_to_reinforce_tower_as_functional_wooden_structure",
        "silhouette": "tower_should_read_as_a_compact_magical_weapon_emplacement",
        "constraint": "improvements_must_feel_like_a_natural_part_of_the_existing_scene_not_a_different_art_style"
      },
      "preserve": {
        "overall_aesthetic": "EXACT_MATCH_keep_the_same_color_mood_art_style_and_visual_tone",
        "background": "EXACT_MATCH",
        "surrounding_elements": "EXACT_MATCH",
        "ground_tiles": "EXACT_MATCH",
        "overall_composition": "EXACT_MATCH",
        "palette_harmony": "EXACT_MATCH_tower_colors_must_stay_consistent_with_scene_palette",
        "art_style": "EXACT_MATCH",
        "other_objects": "DO_NOT_MODIFY"
      }
    }
  }
