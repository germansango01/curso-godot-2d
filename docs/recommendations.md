## Estructura recomendada de carpetas para un proyecto Godot 2D

```
project_root/
├── assets/
│   ├── sprites/
│   │   ├── player/
│   │   ├── enemies/
│   │   ├── items/
│   │   └── ui/
│   ├── audio/
│   │   ├── sfx/
│   │   └── music/
│   ├── fonts/
│   └── tilesets/
│
├── scenes/
│   ├── templates/                       # escenas base (plantillas)
│   │   ├── player_base.tscn
│   │   ├── enemy_base.tscn
│   │   ├── npc_base.tscn
│   │   ├── projectile_base.tscn
│   │   ├── item_base.tscn
│   │   └── level_base.tscn
│   │
│   ├── players/                          # instancias concretas
│   │   └── player_guy.tscn
│   ├── enemies/
│   │   ├── enemy_slime.tscn
│   │   └── enemy_flying.tscn
│   ├── items/
│   │   └── coin.tscn
│   ├── levels/
│   │   ├── level_01.tscn
│   │   └── level_tutorial.tscn
│   └── ui/
│       ├── hud.tscn
│       └── pause_menu.tscn
│
├── scripts/
│   ├── core/                            # sistemas globales / singletons
│   │   ├── game_manager.gd
│   │   ├── save_manager.gd
│   │   └── audio_manager.gd
│   ├── player/
│   │   ├── player_controller.gd
│   │   └── player_stats.gd
│   ├── enemy/
│   │   ├── enemy_ai.gd
│   │   └── enemy_stats.gd
│   ├── items/
│   │   └── collectible.gd
│   └── utils/
│       ├── math_utils.gd
│       └── state_machine.gd
│
├── addons/                              # plugins o herramientas personalizadas
│
├── ui/                                  # assets UI editables (scenes, svg)
│
├── tests/                               # pruebas unitarias / escenas de test
│   └── test_player_movement.tscn
│
├── docs/
│   ├── design.md
│   └── readme_project.md
│
├── builds/                              # exports / distribuciones
│
├── .godot/                              # settings locales (opcional)
├── project.godot
└── .gitignore
```