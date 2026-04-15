machines_awakening/                 # 项目根目录
├── assets/                         # 原始资源文件（搭档工作区）
│   ├── art/                        # 像素画源文件 (Aseprite/PSD)
│   │   ├── characters/             # 角色动画源文件
│   │   ├── environment/            # 环境素材（传送带、机械臂等）
│   │   ├── ui/                     # UI 素材（按钮、面板）
│   │   └── tilesets/               # 瓦片地图源文件
│   └── audio/                      # 音频源文件
│       ├── sfx/                    # 音效
│       └── music/                  # 背景音乐
│
├── game/                           # Godot 项目主目录
│   ├── scenes/                     # 所有场景文件
│   │   ├── main.tscn               # 主场景（入口）
│   │   ├── level_1.tscn            # 关卡1
│   │   ├── level_2.tscn            # 关卡2
│   │   ├── level_3.tscn            # 关卡3
│   │   └── ui/
│   │       ├── main_menu.tscn      # 主菜单
│   │       ├── hacking_ui.tscn     # 黑入界面
│   │       └── dialogue_box.tscn   # 对话界面
│   │
│   ├── scripts/                    # 所有脚本（你的核心工作区）
│   │   ├── core/                   # 核心系统
│   │   │   ├── game_manager.gd     # 游戏状态管理
│   │   │   ├── level_manager.gd    # 关卡切换与数据
│   │   │   ├── save_system.gd      # 存档系统
│   │   │   └── event_bus.gd        # 全局信号总线
│   │   │
│   │   ├── player/                 # 玩家相关
│   │   │   ├── player.gd           # 玩家主逻辑
│   │   │   ├── player_stats.gd     # 能量值、能力解锁
│   │   │   └── hacker_component.gd # 黑入能力组件
│   │   │
│   │   ├── machines/               # 可交互机器
│   │   │   ├── base_machine.gd     # 机器基类
│   │   │   ├── robot_arm.gd        # 机械臂
│   │   │   ├── cctv.gd             # 监控探头
│   │   │   ├── conveyor.gd         # 传送带
│   │   │   ├── door_control.gd     # 门禁控制器
│   │   │   └── terminal.gd         # 剧情终端
│   │   │
│   │   ├── npc/                    # 非玩家角色
│   │   │   ├── base_npc.gd         # NPC 基类
│   │   │   ├── worker.gd           # 工人（巡逻/追踪）
│   │   │   ├── security.gd         # 安保（更警觉）
│   │   │   └── npc_state_machine.gd # NPC 状态机
│   │   │
│   │   ├── ui/                     # UI 脚本
│   │   │   ├── hacking_panel.gd    # 黑入面板
│   │   │   ├── energy_bar.gd       # 能量条
│   │   │   └── dialogue_manager.gd # 对话管理
│   │   │
│   │   ├── utils/                  # 工具类
│   │   │   ├── astar.gd            # A* 寻路算法
│   │   │   ├── raycast.gd          # 视线检测工具
│   │   │   └── json_loader.gd      # JSON 关卡加载器
│   │   │
│   │   └── data/                   # 数据定义
│   │       ├── machine_data.gd     # 机器数据资源
│   │       ├── npc_data.gd         # NPC 数据资源
│   │       └── level_data.gd       # 关卡数据资源
│   │
│   ├── resources/                  # Godot 资源文件
│   │   ├── fonts/                  # 像素字体
│   │   ├── shaders/                # 着色器（扫描线、光效）
│   │   └── levels/                 # JSON 关卡数据
│   │       ├── level_1.json
│   │       ├── level_2.json
│   │       └── level_3.json
│   │
│   ├── textures/                   # 导入后的纹理
│   │   ├── characters/
│   │   ├── environment/
│   │   ├── tilesets/
│   │   └── ui/
│   │
│   ├── audio/                      # 导入后的音频
│   │   ├── sfx/
│   │   └── music/
│   │
│   └── project.godot               # 项目配置文件
│
├── docs/                           # 文档
│   ├── game_design_document.md     # 游戏设计文档
│   ├── narrative_outline.md        # 剧情大纲
│   └── level_design_template.md    # 关卡设计模板
│
└── README.md                       # 项目说明