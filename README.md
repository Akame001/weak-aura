{
  "c": [
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "alpha": 1,
      "anchorFrameType": "SCREEN",
      "anchorPoint": "CENTER",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [],
      "backdropColor": [
        1,
        1,
        1,
        0.5
      ],
      "border": false,
      "borderBackdrop": "Blizzard Tooltip",
      "borderColor": [
        0,
        0,
        0,
        1
      ],
      "borderEdge": "Square Full White",
      "borderInset": 1,
      "borderOffset": 4,
      "borderSize": 2,
      "conditions": [],
      "config": [],
      "controlledChildren": [
        "CornerPosition",
        "PaperDollAnchor",
        "Tracker Background",
        "Hunter Color"
      ],
      "frameStrata": 1,
      "groupIcon": 132996,
      "id": "Config",
      "information": {
        "forceEvents": true
      },
      "internalVersion": 79,
      "load": {
        "class": {
          "multi": []
        },
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        }
      },
      "parent": "Mage Buff & Consumes",
      "regionType": "group",
      "scale": 1,
      "selfPoint": "CENTER",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [],
      "tocversion": 11505,
      "triggers": [
        {
          "trigger": {
            "debuffType": "HELPFUL",
            "event": "Health",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player"
          },
          "untrigger": []
        }
      ],
      "uid": "zIeqXjjNa9w",
      "url": "https://wago.io/rGIX20sGW/3",
      "version": 3,
      "wagoID": "rGIX20sGW",
      "xOffset": 0,
      "yOffset": 0
    },
    {
      "actions": {
        "finish": {
          "custom": "aura_env.frameActivated= false",
          "do_custom": false
        },
        "init": {
          "custom": "if not aura_env.region._mouseoverFrameBckground then\n    aura_env.region._mouseoverFrameBckground = CreateFrame(\"FRAME\", nil, WeakAurasFrame)\nend\nlocal frame = aura_env.region._mouseoverFrameBckground\nframe:SetAllPoints(aura_env.region)\nframe:SetScript(\"OnEnter\", function() WeakAuras.ScanEvents(\"_mouseoverFrameBckground_event\", true) end)\nframe:SetScript(\"OnLeave\", function() WeakAuras.ScanEvents(\"_mouseoverFrameBckground_event\", false) end)\nframe:SetMouseClickEnabled(false)",
          "do_custom": false
        },
        "start": {
          "custom": "aura_env.frameActivated= true",
          "do_custom": false
        }
      },
      "alpha": 1,
      "anchorFrameFrame": "PaperDollFrame",
      "anchorFrameType": "SCREEN",
      "anchorPoint": "TOPRIGHT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "blendMode": "BLEND",
      "color": [
        0.054901960784314,
        0.054901960784314,
        0.054901960784314,
        0
      ],
      "conditions": [],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "customAnchor": "",
      "desaturate": false,
      "discrete_rotation": 0,
      "frameStrata": 2,
      "height": 10,
      "id": "CornerPosition",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "mirror": false,
      "parent": "Config",
      "regionType": "texture",
      "rotate": true,
      "rotation": 0,
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "border_color": [
            0,
            0,
            0,
            1
          ],
          "border_edge": "Square Full White",
          "border_offset": 0,
          "border_size": 1,
          "border_visible": false,
          "type": "subborder"
        }
      ],
      "texture": "Interface\\AddOns\\WeakAuras\\Media\\Textures\\Square_FullWhite",
      "textureWrapMode": "CLAMP",
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "check": "event",
            "custom_hide": "timed",
            "custom_type": "status",
            "debuffType": "HELPFUL",
            "duration": "",
            "dynamicDuration": false,
            "event": "Conditions",
            "events": "_FrameClick",
            "names": [],
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "unit",
            "unevent": "auto",
            "unit": "player",
            "use_alwaystrue": true,
            "use_spellName": true,
            "use_unit": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "customTriggerLogic": "function(trigger)\n    if(aura_env.config.quickTrack) then\n        aura_env.region:SetOffset(200,0)\n    end\n    return trigger[1]\nend",
        "disjunctive": "custom"
      },
      "uid": "B1duHvclWZ7",
      "url": "https://wago.io/rGIX20sGW/3",
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 200,
      "xOffset": 0,
      "yOffset": 0
    },
    {
      "actions": {
        "finish": {
          "custom": "aura_env.frameActivated= false",
          "do_custom": false
        },
        "init": {
          "custom": "if not aura_env.region._mouseoverFrameBckground then\n    aura_env.region._mouseoverFrameBckground = CreateFrame(\"FRAME\", nil, WeakAurasFrame)\nend\nlocal frame = aura_env.region._mouseoverFrameBckground\nframe:SetAllPoints(aura_env.region)\nframe:SetScript(\"OnEnter\", function() WeakAuras.ScanEvents(\"_mouseoverFrameBckground_event\", true) end)\nframe:SetScript(\"OnLeave\", function() WeakAuras.ScanEvents(\"_mouseoverFrameBckground_event\", false) end)\nframe:SetMouseClickEnabled(false)",
          "do_custom": false
        },
        "start": {
          "custom": "aura_env.frameActivated= true",
          "do_custom": false
        }
      },
      "alpha": 1,
      "anchorFrameFrame": "PaperDollFrame",
      "anchorFrameType": "SCREEN",
      "anchorPoint": "TOPRIGHT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "blendMode": "BLEND",
      "color": [
        0.054901960784314,
        0.054901960784314,
        0.054901960784314,
        0
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "xOffsetRelative",
              "value": 180
            },
            {
              "property": "yOffsetRelative",
              "value": -1
            }
          ],
          "check": {
            "trigger": -1,
            "value": "-- Extended Character Stats\nfunction()\n    return aura_env.config.StatsAnchor == 2\nend",
            "variable": "customcheck"
          }
        },
        {
          "changes": [
            {
              "property": "xOffsetRelative",
              "value": 209
            }
          ],
          "check": {
            "trigger": -1,
            "value": "-- WrathArmory\nfunction()\n    return aura_env.config.StatsAnchor == 3\nend",
            "variable": "customcheck"
          }
        },
        {
          "changes": [
            {
              "property": "xOffsetRelative",
              "value": 410
            }
          ],
          "check": {
            "trigger": -1,
            "value": "-- WrathArmory\nfunction()\n    return aura_env.config.StatsAnchor == 4\n\nend",
            "variable": "customcheck"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "customAnchor": "",
      "desaturate": false,
      "discrete_rotation": 0,
      "frameStrata": 2,
      "height": 10,
      "id": "PaperDollAnchor",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "mirror": false,
      "parent": "Config",
      "regionType": "texture",
      "rotate": true,
      "rotation": 0,
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "border_color": [
            0,
            0,
            0,
            1
          ],
          "border_edge": "Square Full White",
          "border_offset": 0,
          "border_size": 1,
          "border_visible": false,
          "type": "subborder"
        }
      ],
      "texture": "Interface\\AddOns\\WeakAuras\\Media\\Textures\\Square_FullWhite",
      "textureWrapMode": "CLAMP",
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "check": "event",
            "custom_hide": "timed",
            "custom_type": "status",
            "debuffType": "HELPFUL",
            "duration": "",
            "dynamicDuration": false,
            "event": "Conditions",
            "events": "_FrameClick",
            "names": [],
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "unit",
            "unevent": "auto",
            "unit": "player",
            "use_alwaystrue": true,
            "use_spellName": true,
            "use_unit": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "customTriggerLogic": "function(trigger)\n    return trigger[2]\nend",
        "disjunctive": "any"
      },
      "uid": "trEga4bwvQA",
      "url": "https://wago.io/rGIX20sGW/3",
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 200,
      "xOffset": 143.89999237061,
      "yOffset": -116.3
    },
    {
      "actions": {
        "finish": {
          "custom": "aura_env.frameActivated= false",
          "do_custom": false
        },
        "init": {
          "custom": "consumablesFrameActive = false",
          "do_custom": false
        },
        "start": {
          "custom": "aura_env.frameActivated= true",
          "do_custom": false
        }
      },
      "alpha": 0.8,
      "anchorFrameType": "CUSTOM",
      "anchorPoint": "TOP",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "blendMode": "BLEND",
      "color": [
        0.054901960784314,
        0.054901960784314,
        0.054901960784314,
        1
      ],
      "conditions": [],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "customAnchor": "",
      "desaturate": false,
      "discrete_rotation": 0,
      "frameStrata": 4,
      "height": 423,
      "id": "Tracker Background",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "mirror": false,
      "parent": "Config",
      "regionType": "texture",
      "rotate": true,
      "rotation": 0,
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "border_color": [
            0,
            0,
            0,
            1
          ],
          "border_edge": "1 Pixel",
          "border_offset": 0,
          "border_size": 1,
          "border_visible": true,
          "type": "subborder"
        }
      ],
      "texture": "Interface\\AddOns\\WeakAuras\\Media\\Textures\\Square_FullWhite",
      "textureWrapMode": "CLAMP",
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "check": "event",
            "custom_hide": "timed",
            "custom_type": "status",
            "debuffType": "HELPFUL",
            "duration": "",
            "dynamicDuration": false,
            "event": "Conditions",
            "events": "_FrameClick",
            "names": [],
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "unit",
            "unevent": "auto",
            "unit": "player",
            "use_alwaystrue": true,
            "use_spellName": true,
            "use_unit": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "customTriggerLogic": "function(trigger)\n    return trigger[2]\nend",
        "disjunctive": "any"
      },
      "uid": "jLn05cpTXVS",
      "url": "https://wago.io/rGIX20sGW/3",
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 199.99998474121,
      "xOffset": 209.76370611191,
      "yOffset": -2.264892578125
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Tracker Background",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "CENTER",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [],
      "blendMode": "BLEND",
      "color": [
        0.1803921610117,
        0.43137258291245,
        0.95294123888016,
        1
      ],
      "conditions": [],
      "config": [],
      "customAnchor": "",
      "desaturate": false,
      "frameStrata": 1,
      "height": 4,
      "id": "Hunter Color",
      "information": [],
      "internalVersion": 79,
      "load": {
        "class": {
          "multi": []
        },
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        }
      },
      "mirror": false,
      "parent": "Config",
      "regionType": "texture",
      "rotate": false,
      "rotation": 0,
      "selfPoint": "CENTER",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "border_color": [
            0,
            0,
            0,
            1
          ],
          "border_edge": "Square Full White",
          "border_offset": 0,
          "border_size": 1,
          "border_visible": true,
          "type": "subborder"
        }
      ],
      "texture": "Interface\\AddOns\\WeakAuras\\Media\\Textures\\Square_FullWhite",
      "textureWrapMode": "CLAMPTOBLACKADDITIVE",
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "debuffType": "HELPFUL",
            "event": "Health",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player"
          },
          "untrigger": []
        },
        "activeTriggerMode": -10
      },
      "uid": "opXj7y3jN7D",
      "url": "https://wago.io/rGIX20sGW/3",
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 200,
      "xOffset": 0,
      "yOffset": 212.22940648216
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "alpha": 1,
      "anchorFrameType": "SCREEN",
      "anchorPoint": "CENTER",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [],
      "backdropColor": [
        1,
        1,
        1,
        0.5
      ],
      "border": false,
      "borderBackdrop": "Blizzard Tooltip",
      "borderColor": [
        0,
        0,
        0,
        1
      ],
      "borderEdge": "Square Full White",
      "borderInset": 1,
      "borderOffset": 4,
      "borderSize": 2,
      "conditions": [],
      "config": [],
      "controlledChildren": [
        "Header: Consumables Background",
        "Header: Consumables",
        "Consumables Group"
      ],
      "frameStrata": 1,
      "groupIcon": 134740,
      "id": "Consumables",
      "information": {
        "forceEvents": true
      },
      "internalVersion": 79,
      "load": {
        "class": {
          "multi": []
        },
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        }
      },
      "parent": "Mage Buff & Consumes",
      "regionType": "group",
      "scale": 1,
      "selfPoint": "CENTER",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [],
      "tocversion": 11505,
      "triggers": [
        {
          "trigger": {
            "debuffType": "HELPFUL",
            "event": "Health",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player"
          },
          "untrigger": []
        }
      ],
      "uid": "71cuaT(xqeI",
      "url": "https://wago.io/rGIX20sGW/3",
      "version": 3,
      "wagoID": "rGIX20sGW",
      "xOffset": 0,
      "yOffset": 0
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "alpha": 0.8,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameParent": true,
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "CENTER",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "blendMode": "BLEND",
      "color": [
        0.054901960784314,
        0.054901960784314,
        0.054901960784314,
        0.95000000298023
      ],
      "conditions": [],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "customAnchor": "",
      "desaturate": false,
      "discrete_rotation": 0,
      "frameStrata": 4,
      "height": 19,
      "id": "Header: Consumables Background",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "mirror": false,
      "parent": "Consumables",
      "regionType": "texture",
      "rotate": true,
      "rotation": 0,
      "selfPoint": "CENTER",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "border_color": [
            0,
            0,
            0,
            1
          ],
          "border_edge": "Square Full White",
          "border_offset": 0,
          "border_size": 1,
          "border_visible": true,
          "type": "subborder"
        }
      ],
      "texture": "Interface\\AddOns\\WeakAuras\\Media\\Textures\\Square_FullWhite",
      "textureWrapMode": "CLAMP",
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Conditions",
            "names": [],
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "unit",
            "unevent": "auto",
            "unit": "player",
            "use_alwaystrue": true,
            "use_spellName": true,
            "use_unit": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10
      },
      "uid": "2j9Ko)HdrQD",
      "url": "https://wago.io/rGIX20sGW/3",
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 200,
      "xOffset": 0.88888893127441,
      "yOffset": 0
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "anchorFrameFrame": "WeakAuras:Tracker Background",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "TOP",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "automaticWidth": "Fixed",
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "customAnchor": "",
      "customTextUpdate": "update",
      "displayText": "Consumables",
      "fixedWidth": 200,
      "font": "Gilroy Bold",
      "fontSize": 12,
      "frameStrata": 4,
      "id": "Header: Consumables",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "justify": "CENTER",
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "outline": "OUTLINE",
      "parent": "Consumables",
      "regionType": "text",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "shadowColor": [
        0,
        0,
        0,
        1
      ],
      "shadowXOffset": 1,
      "shadowYOffset": -1,
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Conditions",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "unit",
            "unevent": "auto",
            "unit": "player",
            "use_alwaystrue": true,
            "use_unit": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10
      },
      "uid": "mwiGaNutuMl",
      "url": "https://wago.io/rGIX20sGW/3",
      "version": 3,
      "wagoID": "rGIX20sGW",
      "wordWrap": "WordWrap",
      "xOffset": -0.21145019531264,
      "yOffset": -2.6666546291777
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "CENTER",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [],
      "backdropColor": [
        1,
        1,
        1,
        0.5
      ],
      "border": false,
      "borderBackdrop": "Blizzard Tooltip",
      "borderColor": [
        0,
        0,
        0,
        1
      ],
      "borderEdge": "Square Full White",
      "borderInset": 1,
      "borderOffset": 4,
      "borderSize": 2,
      "conditions": [],
      "config": [],
      "controlledChildren": [
        "Consumables: Group - In Raid",
        "Consumables: Group - Out of Raid"
      ],
      "frameStrata": 1,
      "groupIcon": 236878,
      "id": "Consumables Group",
      "information": {
        "forceEvents": true
      },
      "internalVersion": 79,
      "load": {
        "class": {
          "multi": []
        },
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        }
      },
      "parent": "Consumables",
      "regionType": "group",
      "scale": 1,
      "selfPoint": "CENTER",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [],
      "tocversion": 11505,
      "triggers": [
        {
          "trigger": {
            "debuffType": "HELPFUL",
            "event": "Health",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player"
          },
          "untrigger": []
        }
      ],
      "uid": "tk2HLeRZgdw",
      "url": "https://wago.io/rGIX20sGW/3",
      "version": 3,
      "wagoID": "rGIX20sGW",
      "xOffset": -90.881704616547,
      "yOffset": -10.881704628949
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "align": "CENTER",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SCREEN",
      "anchorPoint": "CENTER",
      "animate": false,
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "arcLength": 360,
      "authorOptions": [],
      "backdropColor": [
        1,
        1,
        1,
        0.5
      ],
      "border": false,
      "borderBackdrop": "Blizzard Tooltip",
      "borderColor": [
        0,
        0,
        0,
        1
      ],
      "borderEdge": "Square Full White",
      "borderInset": 1,
      "borderOffset": 4,
      "borderSize": 2,
      "centerType": "LR",
      "columnSpace": 1,
      "conditions": [],
      "config": [],
      "constantFactor": "RADIUS",
      "controlledChildren": [
        "Consumables: Flask",
        "Consumable: Oil",
        "Consumables: Elixir of Fortitude",
        "Consumables: Mongoose Elixir",
        "Consumables: Greater Arcane Elixir",
        "Consumables: Elixir of Firepower",
        "Consumables: Elixir of Greater Intellect",
        "Consumables: Food",
        "Consumables: Drink"
      ],
      "frameStrata": 1,
      "fullCircle": true,
      "gridType": "RD",
      "gridWidth": 5,
      "groupIcon": 135991,
      "grow": "DOWN",
      "id": "Consumables: Group - In Raid",
      "information": {
        "forceEvents": true
      },
      "internalVersion": 79,
      "limit": 5,
      "load": {
        "class": {
          "multi": []
        },
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        }
      },
      "parent": "Consumables Group",
      "radius": 200,
      "regionType": "dynamicgroup",
      "rotation": 0,
      "rowSpace": 1,
      "scale": 1,
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "sort": "none",
      "sortHybridTable": {
        "Consumable: Oil": false,
        "Consumables: Drink": false,
        "Consumables: Elixir of Firepower": false,
        "Consumables: Elixir of Fortitude": false,
        "Consumables: Elixir of Greater Intellect": false,
        "Consumables: Flask": false,
        "Consumables: Food": false,
        "Consumables: Greater Arcane Elixir": false,
        "Consumables: Mongoose Elixir": false
      },
      "source": "import",
      "space": 0,
      "stagger": 0,
      "stepAngle": 15,
      "subRegions": [],
      "tocversion": 11505,
      "triggers": [
        {
          "trigger": {
            "debuffType": "HELPFUL",
            "event": "Health",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player"
          },
          "untrigger": []
        }
      ],
      "uid": "OKoUVqcFBg7",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAnchorPerUnit": false,
      "useLimit": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "xOffset": 0,
      "yOffset": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Atal'al Mojo of War\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "show"
          }
        },
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                1,
                0.64705882352941,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "op": "<",
                "trigger": 1,
                "value": "300",
                "variable": "expirationTime"
              },
              {
                "op": ">",
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "op": "<",
            "trigger": -2,
            "variable": "AND"
          }
        },
        {
          "changes": [
            {
              "property": "sub.4.text_visible"
            },
            {
              "property": "sub.5.text_visible"
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "show"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 134821,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 0,
      "id": "Consumables: Flask",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - In Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Flask",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%1.p",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%2.p",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 170,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%3.p",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_3.p_format": "timed",
          "text_text_format_3.p_time_dynamic_threshold": 60,
          "text_text_format_3.p_time_format": 0,
          "text_text_format_3.p_time_legacy_floor": false,
          "text_text_format_3.p_time_mod_rate": true,
          "text_text_format_3.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [
              "Well Fed"
            ],
            "auraspellids": [
              "17628",
              "13512"
            ],
            "debuffType": "HELPFUL",
            "event": "Health",
            "matchesShowOn": "showOnActive",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 13512,
            "realSpellName": 0,
            "spellName": 0,
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "xeLdQnUoXp9",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")\nend\n\nStaticPopupDialogs[\"CONFIRMATION\"] = {\n    text = \"Hold modifier while clicking to use Flask.\",\n    button1 = \"Okay\",\n    timeout = 0,\n    whileDead = true,\n    hideOnEscape = true,\n    preferredIndex = 3,\n}\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\", 150, 0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\n\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Lesser Wizard Oil\n/use 16\n/click StaticPopup1Button2\n]])\n\n-- /script StaticPopup_Show (\"CONFIRMATION\")",
          "do_custom": true
        },
        "start": {
          "custom": "local r = WeakAuras.regions['Mongoose'].region\nlocal btn = CreateFrame(\"Button\", \"mongooseButton\", r, \"SecureActionButtonTemplate\")\nlocal macroText = [[\n/use Elixir of the Mongoose\n]]\n\nbtn:SetAllPoints()\nbtn:SetAttribute(\"type\", \"macro\")\nbtn:SetAttribute(\"macrotext\", macroText:trim():gsub(\"%s+\", \" \"):gsub(\" /\", \"\\n/\"))",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": true,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "show"
          }
        },
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                1,
                0.64705882352941,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "op": "<",
                "trigger": 1,
                "value": "300",
                "variable": "expirationTime"
              },
              {
                "op": ">",
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "op": "<",
            "trigger": -2,
            "variable": "AND"
          }
        },
        {
          "changes": [
            {
              "property": "sub.3.text_visible"
            },
            {
              "property": "sub.5.text_visible"
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "show"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": "134879",
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 0,
      "id": "Consumable: Oil",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true,
            "WARLOCK": true,
            "WARRIOR": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": true,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - In Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Oil ",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%2.p",
          "text_text_format_1.itemCount_format": "none",
          "text_text_format_1.maxUnitCount_format": "none",
          "text_text_format_1.unitCount_format": "none",
          "text_text_format_2.itemCount_format": "none",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_2.unitCount_format": "none",
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%1.p",
          "text_text_format_1.itemCount_format": "none",
          "text_text_format_1.maxUnitCount_format": "none",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_1.unitCount_format": "none",
          "text_text_format_2.itemCount_format": "none",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_2.unitCount_format": "none",
          "text_text_format_3.p_format": "timed",
          "text_text_format_3.p_time_dynamic_threshold": 60,
          "text_text_format_3.p_time_format": 0,
          "text_text_format_3.p_time_legacy_floor": false,
          "text_text_format_3.p_time_mod_rate": true,
          "text_text_format_3.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 170,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "(%3.p)",
          "text_text_format_1.itemCount_format": "none",
          "text_text_format_1.maxUnitCount_format": "none",
          "text_text_format_1.unitCount_format": "none",
          "text_text_format_2.itemCount_format": "none",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_2.unitCount_format": "none",
          "text_text_format_3.p_format": "timed",
          "text_text_format_3.p_time_dynamic_threshold": 60,
          "text_text_format_3.p_time_format": 0,
          "text_text_format_3.p_time_legacy_floor": false,
          "text_text_format_3.p_time_mod_rate": true,
          "text_text_format_3.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": false,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auraspellids": [
              "430585"
            ],
            "debuffType": "HELPFUL",
            "event": "Weapon Enchant",
            "genericShowOn": "showOnCooldown",
            "itemName": 0,
            "matchesShowOn": "showOnActive",
            "names": [],
            "showOn": "showOnActive",
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unit": "player",
            "useExactSpellId": true,
            "use_enchant": false,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_remaining": false,
            "use_showOn": true,
            "use_weapon": true,
            "weapon": "main"
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 20746,
            "realSpellName": 0,
            "spellName": 0,
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_includeCharges": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "3": {
          "trigger": {
            "debuffType": "HELPFUL",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 20746,
            "type": "item",
            "unit": "player",
            "use_count": false,
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_includeCharges": false,
            "use_itemName": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "customTriggerLogic": "",
        "disjunctive": "any"
      },
      "uid": "nFwhb9hxsDT",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Arcane Elixir\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "show"
          }
        },
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                1,
                0.64705882352941,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "op": "<",
                "trigger": 1,
                "value": "300",
                "variable": "expirationTime"
              },
              {
                "op": ">",
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "op": "<",
            "trigger": -2,
            "variable": "AND"
          }
        },
        {
          "changes": [
            {
              "property": "sub.4.text_visible"
            },
            {
              "property": "sub.5.text_visible"
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "show"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 134824,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 2,
      "id": "Consumables: Elixir of Fortitude",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - In Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Elixir of Fortitude",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%1.p",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%2.p",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 170,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%3.p",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_3.p_format": "timed",
          "text_text_format_3.p_time_dynamic_threshold": 60,
          "text_text_format_3.p_time_format": 0,
          "text_text_format_3.p_time_legacy_floor": false,
          "text_text_format_3.p_time_mod_rate": true,
          "text_text_format_3.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [
              "Well Fed"
            ],
            "auraspellids": [
              "3593"
            ],
            "debuffType": "HELPFUL",
            "event": "Health",
            "matchesShowOn": "showOnActive",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 3825,
            "realSpellName": 0,
            "spellName": 0,
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "8bpjvRkczZi",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Elixir of the Mongoose\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "show"
          }
        },
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                1,
                0.64705882352941,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "op": "<",
                "trigger": 1,
                "value": "300",
                "variable": "expirationTime"
              },
              {
                "op": ">",
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "op": "<",
            "trigger": -2,
            "variable": "AND"
          }
        },
        {
          "changes": [
            {
              "property": "sub.4.text_visible"
            },
            {
              "property": "sub.5.text_visible"
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "show"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 134859,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 0,
      "id": "Consumables: Mongoose Elixir",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - In Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Troll's Blood Potion",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%1.p",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%2.p",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 170,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%3.p",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_3.p_format": "timed",
          "text_text_format_3.p_time_dynamic_threshold": 60,
          "text_text_format_3.p_time_format": 0,
          "text_text_format_3.p_time_legacy_floor": false,
          "text_text_format_3.p_time_mod_rate": true,
          "text_text_format_3.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [
              "Well Fed"
            ],
            "auraspellids": [
              "3223"
            ],
            "debuffType": "HELPFUL",
            "event": "Health",
            "matchesShowOn": "showOnActive",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 3826,
            "realSpellName": 0,
            "spellName": 0,
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "tLu)rGglt7Q",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Arcane Elixir\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "show"
          }
        },
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                1,
                0.64705882352941,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "op": "<",
                "trigger": 1,
                "value": "300",
                "variable": "expirationTime"
              },
              {
                "op": ">",
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "op": "<",
            "trigger": -2,
            "variable": "AND"
          }
        },
        {
          "changes": [
            {
              "property": "sub.4.text_visible"
            },
            {
              "property": "sub.5.text_visible"
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "show"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 134805,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 0,
      "id": "Consumables: Greater Arcane Elixir",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - In Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Greater Arcane Elixir",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%1.p",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%2.p",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 170,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%3.p",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_3.p_format": "timed",
          "text_text_format_3.p_time_dynamic_threshold": 60,
          "text_text_format_3.p_time_format": 0,
          "text_text_format_3.p_time_legacy_floor": false,
          "text_text_format_3.p_time_mod_rate": true,
          "text_text_format_3.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [
              "Well Fed"
            ],
            "auraspellids": [
              "17539"
            ],
            "debuffType": "HELPFUL",
            "event": "Health",
            "matchesShowOn": "showOnActive",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 13454,
            "realSpellName": 0,
            "spellName": 0,
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "bQITeBnwCDN",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Elixir of the Mongoose\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "show"
          }
        },
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                1,
                0.64705882352941,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "op": "<",
                "trigger": 1,
                "value": "300",
                "variable": "expirationTime"
              },
              {
                "op": ">",
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "op": "<",
            "trigger": -2,
            "variable": "AND"
          }
        },
        {
          "changes": [
            {
              "property": "sub.4.text_visible"
            },
            {
              "property": "sub.5.text_visible"
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "show"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 134714,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 0,
      "id": "Consumables: Elixir of Firepower",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - In Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Elixir of Frost Power",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%1.p",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%2.p",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 170,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%3.p",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_3.p_format": "timed",
          "text_text_format_3.p_time_dynamic_threshold": 60,
          "text_text_format_3.p_time_format": 0,
          "text_text_format_3.p_time_legacy_floor": false,
          "text_text_format_3.p_time_mod_rate": true,
          "text_text_format_3.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [
              "Well Fed"
            ],
            "auraspellids": [
              "21920"
            ],
            "debuffType": "HELPFUL",
            "event": "Health",
            "matchesShowOn": "showOnActive",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 17708,
            "realSpellName": 0,
            "spellName": 0,
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "RWtEq7HKBh1",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Elixir of the Mongoose\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "show"
          }
        },
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                1,
                0.64705882352941,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "op": "<",
                "trigger": 1,
                "value": "300",
                "variable": "expirationTime"
              },
              {
                "op": ">",
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "op": "<",
            "trigger": -2,
            "variable": "AND"
          }
        },
        {
          "changes": [
            {
              "property": "sub.4.text_visible"
            },
            {
              "property": "sub.5.text_visible"
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "show"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 134721,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 0,
      "id": "Consumables: Elixir of Greater Intellect",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": true,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - In Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Greater Intellect",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%1.p",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%2.p",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 170,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%3.p",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_3.p_format": "timed",
          "text_text_format_3.p_time_dynamic_threshold": 60,
          "text_text_format_3.p_time_format": 0,
          "text_text_format_3.p_time_legacy_floor": false,
          "text_text_format_3.p_time_mod_rate": true,
          "text_text_format_3.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [
              "Well Fed"
            ],
            "auraspellids": [
              "11396"
            ],
            "debuffType": "HELPFUL",
            "event": "Health",
            "matchesShowOn": "showOnActive",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 9179,
            "realSpellName": 0,
            "spellName": 0,
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "13QniN62ygK",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Grilled Squid\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "show"
          }
        },
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                1,
                0.64705882352941,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "op": "<",
                "trigger": 1,
                "value": "300",
                "variable": "expirationTime"
              },
              {
                "op": ">",
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "op": "<",
            "trigger": -2,
            "variable": "AND"
          }
        },
        {
          "changes": [
            {
              "property": "sub.4.text_visible"
            },
            {
              "property": "sub.5.text_visible"
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "show"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": "136000",
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 0,
      "id": "Consumables: Food",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - In Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Food Buff",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%1.p",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%2.p",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 170,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%3.p",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_3.p_format": "timed",
          "text_text_format_3.p_time_dynamic_threshold": 60,
          "text_text_format_3.p_time_format": 0,
          "text_text_format_3.p_time_legacy_floor": false,
          "text_text_format_3.p_time_mod_rate": true,
          "text_text_format_3.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [
              "Well Fed"
            ],
            "auraspellids": [
              "18194"
            ],
            "debuffType": "HELPFUL",
            "event": "Health",
            "matchesShowOn": "showOnActive",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 13931,
            "realSpellName": 0,
            "spellName": 0,
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "CM0v9SvJacH",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Grilled Squid\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "show"
          }
        },
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                1,
                0.64705882352941,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "op": "<",
                "trigger": 1,
                "value": "300",
                "variable": "expirationTime"
              },
              {
                "op": ">",
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "op": "<",
            "trigger": -2,
            "variable": "AND"
          }
        },
        {
          "changes": [
            {
              "property": "sub.4.text_visible"
            },
            {
              "property": "sub.5.text_visible"
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "show"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 132791,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 0,
      "id": "Consumables: Drink",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - In Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Rumsey Rum",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%1.p",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%2.p",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 170,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%3.p",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_3.p_format": "timed",
          "text_text_format_3.p_time_dynamic_threshold": 60,
          "text_text_format_3.p_time_format": 0,
          "text_text_format_3.p_time_legacy_floor": false,
          "text_text_format_3.p_time_mod_rate": true,
          "text_text_format_3.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [
              "Well Fed"
            ],
            "auraspellids": [
              "25804",
              "25722"
            ],
            "debuffType": "HELPFUL",
            "event": "Health",
            "matchesShowOn": "showOnActive",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 21114,
            "realSpellName": 0,
            "spellName": 0,
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "Hq(Uvyuruot",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "align": "CENTER",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SCREEN",
      "anchorPoint": "CENTER",
      "animate": false,
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "arcLength": 360,
      "authorOptions": [],
      "backdropColor": [
        1,
        1,
        1,
        0.5
      ],
      "border": false,
      "borderBackdrop": "Blizzard Tooltip",
      "borderColor": [
        0,
        0,
        0,
        1
      ],
      "borderEdge": "Square Full White",
      "borderInset": 1,
      "borderOffset": 4,
      "borderSize": 2,
      "centerType": "LR",
      "columnSpace": 1,
      "conditions": [],
      "config": [],
      "constantFactor": "RADIUS",
      "controlledChildren": [
        "Consumables: Flask 2",
        "Consumable: Oil 2",
        "Consumables: Elixir of Fortitude 2",
        "Consumables: Greater Arcane Elixir 2",
        "Consumables: Troll's Blood Potion",
        "Consumables: Elixir of Greater Intellect 2",
        "Consumables: Elixir of Frostpower 2",
        "Consumables: Food 2",
        "Consumables: Drink 2",
        "Consumables: Nature Protection Potion 2",
        "Consumables: LIP 2",
        "Consumables: FAP 2",
        "Consumables: Swiftness Potion 2",
        "Consumables: Major Healing Potion 2",
        "Consumables: Heavy Runecloth Bandage 2",
        "Consumables: Goblin Sapper Charge 2",
        "Consumables: Dense Dynamite 2"
      ],
      "frameStrata": 1,
      "fullCircle": true,
      "gridType": "RD",
      "gridWidth": 5,
      "groupIcon": 135991,
      "grow": "DOWN",
      "id": "Consumables: Group - Out of Raid",
      "information": {
        "forceEvents": true
      },
      "internalVersion": 79,
      "limit": 5,
      "load": {
        "class": {
          "multi": []
        },
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        }
      },
      "parent": "Consumables Group",
      "radius": 200,
      "regionType": "dynamicgroup",
      "rotation": 0,
      "rowSpace": 1,
      "scale": 1,
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "sort": "none",
      "sortHybridTable": {
        "Consumable: Oil 2": false,
        "Consumables: Dense Dynamite 2": false,
        "Consumables: Drink 2": false,
        "Consumables: Elixir of Firepower 2": false,
        "Consumables: Elixir of Fortitude 2": false,
        "Consumables: Elixir of Greater Intellect 2": false,
        "Consumables: FAP 2": false,
        "Consumables: Flask 2": false,
        "Consumables: Food 2": false,
        "Consumables: Goblin Sapper Charge 2": false,
        "Consumables: Greater Arcane Elixir 2": false,
        "Consumables: Heavy Runecloth Bandage 2": false,
        "Consumables: LIP 2": false,
        "Consumables: Major Healing Potion 2": false,
        "Consumables: Nature Protection Potion 2": false,
        "Consumables: Swiftness Potion 2": false,
        "Consumables: Troll's Blood Potion": false
      },
      "source": "import",
      "space": 0,
      "stagger": 0,
      "stepAngle": 15,
      "subRegions": [],
      "tocversion": 11505,
      "triggers": [
        {
          "trigger": {
            "debuffType": "HELPFUL",
            "event": "Health",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player"
          },
          "untrigger": []
        }
      ],
      "uid": "Y6rJEYES8)v",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAnchorPerUnit": false,
      "useLimit": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "xOffset": 0,
      "yOffset": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Atal'al Mojo of War\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": false
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0.047058828175068,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "trigger": -2,
            "variable": "OR"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 134821,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 0,
      "id": "Consumables: Flask 2",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "group": true,
            "solo": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - Out of Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Flask",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%s",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "count": "1",
            "count_operator": ">=",
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 13512,
            "names": [],
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_count": true,
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 13512,
            "subeventPrefix": "",
            "subeventSuffix": "",
            "type": "item",
            "unit": "player",
            "use_alwaystrue": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_unit": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "61t3OpMpKpw",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")\nend\n\nStaticPopupDialogs[\"CONFIRMATION\"] = {\n    text = \"Hold modifier while clicking to use Flask.\",\n    button1 = \"Okay\",\n    timeout = 0,\n    whileDead = true,\n    hideOnEscape = true,\n    preferredIndex = 3,\n}\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\", 150, 0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\n\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Lesser Wizard Oil\n/use 16\n/click StaticPopup1Button2\n]])\n\n-- /script StaticPopup_Show (\"CONFIRMATION\")",
          "do_custom": true
        },
        "start": {
          "custom": "local r = WeakAuras.regions['Mongoose'].region\nlocal btn = CreateFrame(\"Button\", \"mongooseButton\", r, \"SecureActionButtonTemplate\")\nlocal macroText = [[\n/use Elixir of the Mongoose\n]]\n\nbtn:SetAllPoints()\nbtn:SetAttribute(\"type\", \"macro\")\nbtn:SetAttribute(\"macrotext\", macroText:trim():gsub(\"%s+\", \" \"):gsub(\" /\", \"\\n/\"))",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": true,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0.047058828175068,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "trigger": -2,
            "variable": "OR"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": "134879",
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 0,
      "id": "Consumable: Oil 2",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true,
            "WARLOCK": true,
            "WARRIOR": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "group": true,
            "solo": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": true,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - Out of Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Oil",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%s",
          "text_text_format_1.itemCount_format": "none",
          "text_text_format_1.maxUnitCount_format": "none",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_1.stacks_format": "none",
          "text_text_format_1.unitCount_format": "none",
          "text_text_format_1p_format": "none",
          "text_text_format_2.itemCount_format": "none",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_2.unitCount_format": "none",
          "text_text_format_3.p_format": "timed",
          "text_text_format_3.p_time_dynamic_threshold": 60,
          "text_text_format_3.p_time_format": 0,
          "text_text_format_3.p_time_legacy_floor": false,
          "text_text_format_3.p_time_mod_rate": true,
          "text_text_format_3.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "count": "1",
            "count_operator": ">=",
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 20746,
            "names": [],
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_count": true,
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_includeCharges": false,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 20746,
            "type": "item",
            "unit": "player",
            "use_genericShowOn": true,
            "use_itemName": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "customTriggerLogic": "",
        "disjunctive": "any"
      },
      "uid": "6)bVyomlfUf",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Arcane Elixir\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": false
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0.0039215688593686,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "trigger": -2,
            "variable": "OR"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 134824,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": -1,
      "id": "Consumables: Elixir of Fortitude 2",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "group": true,
            "solo": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - Out of Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Elixir of Fortitude",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%s",
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 60,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": false,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "count": "10",
            "count_operator": ">=",
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 3825,
            "names": [],
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_count": true,
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 3825,
            "type": "item",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "z20EW05pL80",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Arcane Elixir\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0.0039215688593686,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "trigger": -2,
            "variable": "OR"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 134805,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 0,
      "id": "Consumables: Greater Arcane Elixir 2",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "group": true,
            "solo": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - Out of Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Greater Arcane Elixir",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%s",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [
              "Well Fed"
            ],
            "auraspellids": [
              "17539"
            ],
            "count": "10",
            "count_operator": ">=",
            "debuffType": "HELPFUL",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 13454,
            "matchesShowOn": "showOnActive",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unit": "player",
            "useExactSpellId": true,
            "use_count": true,
            "use_genericShowOn": true,
            "use_itemName": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 13454,
            "names": [],
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "ehNS8IXW63T",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Elixir of the Mongoose\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0.047058828175068,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "trigger": -2,
            "variable": "OR"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 134859,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 0,
      "id": "Consumables: Troll's Blood Potion",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "group": true,
            "solo": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - Out of Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Troll's Blood Potion",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%s",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [
              "Well Fed"
            ],
            "auraspellids": [
              "3223"
            ],
            "count": "10",
            "count_operator": ">=",
            "debuffType": "HELPFUL",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 3826,
            "matchesShowOn": "showOnActive",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unit": "player",
            "useExactSpellId": true,
            "use_count": true,
            "use_genericShowOn": true,
            "use_itemName": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 3826,
            "realSpellName": 0,
            "spellName": 0,
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "W1IgKNrOj0u",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Elixir of the Mongoose\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0.047058828175068,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "trigger": -2,
            "variable": "OR"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 134827,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": -1,
      "id": "Consumables: Elixir of Greater Intellect 2",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "group": true,
            "solo": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - Out of Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Major Mana Potion",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%s",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [
              "Well Fed"
            ],
            "auraspellids": [
              "11396"
            ],
            "count": "20",
            "count_operator": ">=",
            "debuffType": "HELPFUL",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 13444,
            "matchesShowOn": "showOnActive",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unit": "player",
            "useExactSpellId": true,
            "use_count": true,
            "use_genericShowOn": true,
            "use_itemName": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 13444,
            "realSpellName": 0,
            "spellName": 0,
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "Job3sxP(fTF",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Elixir of the Mongoose\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0.047058828175068,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "trigger": -2,
            "variable": "OR"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 134714,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 0,
      "id": "Consumables: Elixir of Frostpower 2",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "group": true,
            "solo": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - Out of Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Elixir of Frost Power",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%s",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [
              "Well Fed"
            ],
            "auraspellids": [
              "7844"
            ],
            "count": "10",
            "count_operator": ">=",
            "debuffType": "HELPFUL",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 17708,
            "matchesShowOn": "showOnActive",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unit": "player",
            "useExactSpellId": true,
            "use_count": true,
            "use_genericShowOn": true,
            "use_itemName": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 17708,
            "realSpellName": 0,
            "spellName": 0,
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "vp9R)nTzxZo",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Grilled Squid\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0.047058828175068,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "trigger": -2,
            "variable": "OR"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": "136000",
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 0,
      "id": "Consumables: Food 2",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "group": true,
            "solo": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - Out of Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Food Buff",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%s",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [
              "Well Fed"
            ],
            "auraspellids": [
              "19709"
            ],
            "count": "20",
            "count_operator": ">=",
            "debuffType": "HELPFUL",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 13931,
            "matchesShowOn": "showOnActive",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unit": "player",
            "useExactSpellId": true,
            "use_count": true,
            "use_genericShowOn": true,
            "use_itemName": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 13931,
            "realSpellName": 0,
            "spellName": 0,
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "cQUfHdBuomz",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Grilled Squid\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0.047058828175068,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "trigger": -2,
            "variable": "OR"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 132791,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 0,
      "id": "Consumables: Drink 2",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "group": true,
            "solo": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - Out of Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Rumsey Rum",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%s",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [
              "Well Fed"
            ],
            "auraspellids": [
              "25804",
              "25722"
            ],
            "count": "10",
            "count_operator": ">=",
            "debuffType": "HELPFUL",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 21114,
            "matchesShowOn": "showOnActive",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unit": "player",
            "useExactSpellId": true,
            "use_count": true,
            "use_genericShowOn": true,
            "use_itemName": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 21114,
            "realSpellName": 0,
            "spellName": 0,
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "c43WBEYfKY1",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Nature Protection Potion\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0.047058828175068,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "trigger": -2,
            "variable": "OR"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 136094,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 2,
      "id": "Consumables: Nature Protection Potion 2",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "group": true,
            "solo": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - Out of Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "GFPP",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%s",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "count": "10",
            "count_operator": ">=",
            "debuffType": "HELPFUL",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 13457,
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unit": "player",
            "use_count": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_remaining": false
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 13457,
            "names": [],
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "dWcMMnkNNHB",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Nature Protection Potion\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0.047058828175068,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "trigger": -2,
            "variable": "OR"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 135896,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 1,
      "id": "Consumables: LIP 2",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "group": true,
            "solo": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - Out of Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "LIP",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%s",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "count": "5",
            "count_operator": ">=",
            "debuffType": "HELPFUL",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 3387,
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unit": "player",
            "use_count": true,
            "use_genericShowOn": true,
            "use_itemName": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 3387,
            "names": [],
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "mADlCVxoS3z",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Nature Protection Potion\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0.047058828175068,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "trigger": -2,
            "variable": "OR"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 134715,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 1,
      "id": "Consumables: FAP 2",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "group": true,
            "solo": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": true,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - Out of Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "FAP",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%s",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "count": "5",
            "count_operator": ">=",
            "debuffType": "HELPFUL",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 5634,
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unit": "player",
            "use_count": true,
            "use_genericShowOn": true,
            "use_itemName": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 5634,
            "names": [],
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "RkHOdVvh3vD",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Nature Protection Potion\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0.047058828175068,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "trigger": -2,
            "variable": "OR"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 134827,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 1,
      "id": "Consumables: Swiftness Potion 2",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "group": true,
            "solo": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": true,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - Out of Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Swiftness Potion",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%s",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "count": "5",
            "count_operator": ">=",
            "debuffType": "HELPFUL",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 2459,
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unit": "player",
            "use_count": true,
            "use_genericShowOn": true,
            "use_itemName": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 2459,
            "names": [],
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "k3RC6JqpSz8",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Nature Protection Potion\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0.047058828175068,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "trigger": -2,
            "variable": "OR"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 134827,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": -1,
      "id": "Consumables: Major Healing Potion 2",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "group": true,
            "solo": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - Out of Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Major Healing Potion",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%s",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "count": "5",
            "count_operator": ">=",
            "debuffType": "HELPFUL",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 13446,
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unit": "player",
            "use_count": true,
            "use_genericShowOn": true,
            "use_itemName": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 13446,
            "names": [],
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "4GIDSt3PTLJ",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Nature Protection Potion\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0.047058828175068,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "trigger": -2,
            "variable": "OR"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 133682,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 1,
      "id": "Consumables: Heavy Runecloth Bandage 2",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "group": true,
            "solo": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - Out of Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Runecloth Bandage",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%s",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "count": "20",
            "count_operator": ">=",
            "debuffType": "HELPFUL",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 14530,
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unit": "player",
            "use_count": true,
            "use_genericShowOn": true,
            "use_itemName": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 14530,
            "names": [],
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "zU5khUfdWmK",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Grilled Squid\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0.047058828175068,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "trigger": 1,
                "value": 1,
                "variable": "show"
              }
            ],
            "trigger": -2,
            "variable": "OR"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 135826,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 0,
      "id": "Consumables: Goblin Sapper Charge 2",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "group": true,
            "solo": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - Out of Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Goblin Sapper Charge",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%s",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "count": "10",
            "count_operator": ">=",
            "debuffType": "HELPFUL",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 10646,
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unit": "player",
            "use_count": true,
            "use_genericShowOn": true,
            "use_itemName": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "count": "20",
            "count_operator": ">=",
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 10646,
            "names": [],
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_count": false,
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "SQvWmLdNUTX",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\n\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/use [nomod] Grilled Squid\n]])\n\n\n\n\n\n--aura_env.clickableFrame:SetScript(\"OnClick\", function() StaticPopup_Show (\"CONFIRMATION\") end)",
          "do_custom": true
        },
        "start": {
          "custom": "\n\n",
          "do_custom": false
        }
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Consumables",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": false,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "value": 1,
            "variable": "show"
          }
        },
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                1,
                0.64705882352941,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "op": "<",
                "value": "300",
                "variable": "expirationTime"
              },
              {
                "op": ">",
                "value": 1,
                "variable": "show"
              }
            ],
            "op": "<",
            "trigger": -2,
            "variable": "AND"
          }
        },
        {
          "changes": [
            [],
            []
          ],
          "check": {
            "value": 1,
            "variable": "show"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 135826,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 1,
      "id": "Consumables: Dense Dynamite 2",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "MAGE": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "group": true,
            "solo": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": false,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Consumables: Group - Out of Raid",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Dense Dynamite",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%s",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": false,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": false,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "count": "10",
            "count_operator": ">=",
            "debuffType": "HELPFUL",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 18641,
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unit": "player",
            "use_count": true,
            "use_genericShowOn": true,
            "use_itemName": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "count": "20",
            "count_operator": ">=",
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "genericShowOn": "showOnCooldown",
            "itemName": 18641,
            "names": [],
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "item",
            "unevent": "auto",
            "unit": "player",
            "use_count": false,
            "use_exact_itemName": true,
            "use_genericShowOn": true,
            "use_itemName": true,
            "use_spellName": true,
            "use_track": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "fuWcxqTTPUN",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "alpha": 1,
      "anchorFrameType": "SCREEN",
      "anchorPoint": "CENTER",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [],
      "backdropColor": [
        1,
        1,
        1,
        0.5
      ],
      "border": false,
      "borderBackdrop": "Blizzard Tooltip",
      "borderColor": [
        0,
        0,
        0,
        1
      ],
      "borderEdge": "Square Full White",
      "borderInset": 1,
      "borderOffset": 4,
      "borderSize": 2,
      "conditions": [],
      "config": [],
      "controlledChildren": [
        "Header: Raid Buffs Background",
        "Header: Raid Buffs",
        "Buffs Group"
      ],
      "frameStrata": 1,
      "groupIcon": 135941,
      "id": "Raid Buffs",
      "information": {
        "forceEvents": true
      },
      "internalVersion": 79,
      "load": {
        "class": {
          "multi": []
        },
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        }
      },
      "parent": "Mage Buff & Consumes",
      "regionType": "group",
      "scale": 1,
      "selfPoint": "CENTER",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [],
      "tocversion": 11505,
      "triggers": [
        {
          "trigger": {
            "debuffType": "HELPFUL",
            "event": "Health",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player"
          },
          "untrigger": []
        }
      ],
      "uid": "wqJ1JOVsndw",
      "url": "https://wago.io/rGIX20sGW/3",
      "version": 3,
      "wagoID": "rGIX20sGW",
      "xOffset": 0,
      "yOffset": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": ""
        },
        "start": []
      },
      "alpha": 0.8,
      "anchorFrameFrame": "WeakAuras:Header: Raid Buffs",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "CENTER",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "blendMode": "BLEND",
      "color": [
        0.054901960784314,
        0.054901960784314,
        0.054901960784314,
        0.95000000298023
      ],
      "conditions": [],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "customAnchor": "",
      "desaturate": false,
      "discrete_rotation": 0,
      "frameStrata": 4,
      "height": 15.842695999145,
      "id": "Header: Raid Buffs Background",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_ingroup": true,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "mirror": false,
      "parent": "Raid Buffs",
      "regionType": "texture",
      "rotate": true,
      "rotation": 0,
      "selfPoint": "CENTER",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "border_color": [
            0,
            0,
            0,
            1
          ],
          "border_edge": "Square Full White",
          "border_offset": 0,
          "border_size": 1,
          "border_visible": true,
          "type": "subborder"
        }
      ],
      "texture": "Interface\\AddOns\\WeakAuras\\Media\\Textures\\Square_FullWhite",
      "textureWrapMode": "CLAMP",
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Conditions",
            "names": [],
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "unit",
            "unevent": "auto",
            "unit": "player",
            "use_alwaystrue": true,
            "use_spellName": true,
            "use_unit": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10
      },
      "uid": "U(249OUTB(n",
      "url": "https://wago.io/rGIX20sGW/3",
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 199.80328063965,
      "xOffset": 10.073624316129,
      "yOffset": 0.98735894097222
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "\n\n",
          "do_custom": false
        },
        "start": []
      },
      "anchorFrameFrame": "WeakAuras:Tracker Background",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "TOP",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "automaticWidth": "Fixed",
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "yOffsetRelative",
              "value": -14
            }
          ],
          "check": {
            "op": "ACTIVE_TALENT_GROUP_CHANGED",
            "trigger": -1,
            "value": "function()\n    local _, _, classIndex = UnitClass(\"player\");\n    \n    -- Paladin\n    if(classIndex == 2) then \n        -- Beacon of Light (Holy Spec)\n        local _, _, _, _, beaconSlct, _, _, _ = GetTalentInfo(1, 23, false);    \n        if(beaconSlct == 1) then\n            return true            \n        else\n            return false\n        end\n    elseif (classIndex == 3) then\n        return true\n    else\n        return false\n    end\nend",
            "variable": "customcheck"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "customAnchor": "",
      "customTextUpdate": "update",
      "displayText": "Raid Buffs",
      "fixedWidth": 200,
      "font": "Gilroy Bold",
      "fontSize": 12,
      "frameStrata": 4,
      "id": "Header: Raid Buffs",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "justify": "CENTER",
      "load": {
        "class": {
          "multi": {
            "DEATHKNIGHT": true,
            "DRUID": true,
            "HUNTER": true,
            "MAGE": true,
            "PRIEST": true,
            "ROGUE": true,
            "SHAMAN": true,
            "WARLOCK": true,
            "WARRIOR": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_ingroup": true,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "outline": "OUTLINE",
      "parent": "Raid Buffs",
      "regionType": "text",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "shadowColor": [
        0,
        0,
        0,
        1
      ],
      "shadowXOffset": 1,
      "shadowYOffset": -1,
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Conditions",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "unit",
            "unevent": "auto",
            "unit": "player",
            "use_alwaystrue": true,
            "use_unit": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "P3c(24gw(7o",
      "url": "https://wago.io/rGIX20sGW/3",
      "version": 3,
      "wagoID": "rGIX20sGW",
      "wordWrap": "WordWrap",
      "xOffset": -9.7777782440186,
      "yOffset": -210.13444444444
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Raid Buffs",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "CENTER",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [],
      "backdropColor": [
        1,
        1,
        1,
        0.5
      ],
      "border": false,
      "borderBackdrop": "Blizzard Tooltip",
      "borderColor": [
        0,
        0,
        0,
        1
      ],
      "borderEdge": "Square Full White",
      "borderInset": 1,
      "borderOffset": 4,
      "borderSize": 2,
      "conditions": [],
      "config": [],
      "controlledChildren": [
        "Buffs: Group - Mage"
      ],
      "frameStrata": 1,
      "groupIcon": 135987,
      "id": "Buffs Group",
      "information": {
        "forceEvents": true
      },
      "internalVersion": 79,
      "load": {
        "class": {
          "multi": []
        },
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        }
      },
      "parent": "Raid Buffs",
      "regionType": "group",
      "scale": 1,
      "selfPoint": "CENTER",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [],
      "tocversion": 11505,
      "triggers": [
        {
          "trigger": {
            "debuffType": "HELPFUL",
            "event": "Health",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player"
          },
          "untrigger": []
        }
      ],
      "uid": "nYIcoxpd3)C",
      "url": "https://wago.io/rGIX20sGW/3",
      "version": 3,
      "wagoID": "rGIX20sGW",
      "xOffset": -81.111110687256,
      "yOffset": -24.111111111111
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "align": "CENTER",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Raid Buffs",
      "anchorFrameType": "SCREEN",
      "anchorPoint": "CENTER",
      "animate": false,
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "arcLength": 360,
      "authorOptions": [],
      "backdropColor": [
        1,
        1,
        1,
        0.5
      ],
      "border": false,
      "borderBackdrop": "Blizzard Tooltip",
      "borderColor": [
        0,
        0,
        0,
        1
      ],
      "borderEdge": "Square Full White",
      "borderInset": 1,
      "borderOffset": 4,
      "borderSize": 2,
      "centerType": "LR",
      "columnSpace": 1,
      "conditions": [],
      "config": [],
      "constantFactor": "RADIUS",
      "controlledChildren": [
        "Fortitude",
        "King  2",
        "Salvation 2",
        "Wisdom 3",
        "Light 3",
        "Spirit 2",
        "Gift of the Wild",
        "Arcane Intellect",
        "Mage Armor"
      ],
      "frameStrata": 1,
      "fullCircle": true,
      "gridType": "RD",
      "gridWidth": 5,
      "groupIcon": 135991,
      "grow": "DOWN",
      "id": "Buffs: Group - Mage",
      "information": {
        "forceEvents": true
      },
      "internalVersion": 79,
      "limit": 5,
      "load": {
        "class": {
          "multi": []
        },
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        }
      },
      "parent": "Buffs Group",
      "radius": 200,
      "regionType": "dynamicgroup",
      "rotation": 0,
      "rowSpace": 1,
      "scale": 1,
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "sort": "none",
      "sortHybridTable": {
        "Arcane Intellect": false,
        "Fortitude": false,
        "Gift of the Wild": false,
        "Molten Armor": false
      },
      "source": "import",
      "space": 0,
      "stagger": 0,
      "stepAngle": 15,
      "subRegions": [],
      "tocversion": 11505,
      "triggers": [
        {
          "trigger": {
            "debuffType": "HELPFUL",
            "event": "Health",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player"
          },
          "untrigger": []
        }
      ],
      "uid": "3LIhVeETkVR",
      "url": "https://wago.io/rGIX20sGW/3",
      "useLimit": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "xOffset": 0,
      "yOffset": 18.666666666667
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r)  \nend\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\n\n\naura_env.clickableFrame:SetScript(\"OnClick\", function()\n        SendChatMessage(\"Please buff Fortitude\", \"RAID\")\n    end\n)",
          "do_custom": true
        },
        "start": []
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Raid Buffs",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": true,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "buffed"
          }
        },
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                1,
                0.64705882352941,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "op": "<",
                "trigger": 1,
                "value": "300",
                "variable": "expirationTime"
              },
              {
                "op": ">",
                "trigger": 1,
                "value": 1,
                "variable": "buffed"
              }
            ],
            "op": "<",
            "trigger": -2,
            "variable": "AND"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 135941,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": -1,
      "id": "Fortitude",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": true,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Buffs: Group - Mage",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Fortitude",
          "text_text_format_n_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%p",
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [],
            "auraspellids": [
              "10937",
              "21564"
            ],
            "debuffType": "HELPFUL",
            "event": "Health",
            "matchesShowOn": "showAlways",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10
      },
      "uid": "7o6vjw7B3pD",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": -2.2222222222222,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r)  \nend\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\n\n\naura_env.clickableFrame:SetScript(\"OnClick\", function()\n        SendChatMessage(\"Please buff Fortitude\", \"RAID\")\n    end\n)",
          "do_custom": true
        },
        "start": []
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Raid Buffs",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": true,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "buffed"
          }
        },
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                1,
                0.64705882352941,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "op": "<",
                "trigger": 1,
                "value": "300",
                "variable": "expirationTime"
              },
              {
                "op": ">",
                "trigger": 1,
                "value": 1,
                "variable": "buffed"
              }
            ],
            "op": "<",
            "trigger": -2,
            "variable": "AND"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 135941,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": -1,
      "id": "King  2",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": true,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Buffs: Group - Mage",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Blessing of Kings",
          "text_text_format_n_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%p",
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [],
            "auraspellids": [
              " 25898"
            ],
            "debuffType": "HELPFUL",
            "event": "Health",
            "matchesShowOn": "showAlways",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10
      },
      "uid": "9Nhc(Ib9Uuc",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": -2.2222222222222,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r)  \nend\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\n\n\naura_env.clickableFrame:SetScript(\"OnClick\", function()\n        SendChatMessage(\"Please buff Fortitude\", \"RAID\")\n    end\n)",
          "do_custom": true
        },
        "start": []
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Raid Buffs",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": true,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "buffed"
          }
        },
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                1,
                0.64705882352941,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "op": "<",
                "trigger": 1,
                "value": "300",
                "variable": "expirationTime"
              },
              {
                "op": ">",
                "trigger": 1,
                "value": 1,
                "variable": "buffed"
              }
            ],
            "op": "<",
            "trigger": -2,
            "variable": "AND"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 135941,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": -1,
      "id": "Salvation 2",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": true,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Buffs: Group - Mage",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Blessing of Salvation",
          "text_text_format_n_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%p",
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [],
            "auraspellids": [
              "25895"
            ],
            "debuffType": "HELPFUL",
            "event": "Health",
            "matchesShowOn": "showAlways",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10
      },
      "uid": "N8GsM(Z9fMW",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": -2.2222222222222,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r)  \nend\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\n\n\naura_env.clickableFrame:SetScript(\"OnClick\", function()\n        SendChatMessage(\"Please buff Fortitude\", \"RAID\")\n    end\n)",
          "do_custom": true
        },
        "start": []
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Raid Buffs",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": true,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "buffed"
          }
        },
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                1,
                0.64705882352941,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "op": "<",
                "trigger": 1,
                "value": "300",
                "variable": "expirationTime"
              },
              {
                "op": ">",
                "trigger": 1,
                "value": 1,
                "variable": "buffed"
              }
            ],
            "op": "<",
            "trigger": -2,
            "variable": "AND"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 135941,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": -1,
      "id": "Wisdom 3",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": true,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Buffs: Group - Mage",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Blessing of Wisdom",
          "text_text_format_n_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%p",
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [],
            "auraspellids": [
              "25894"
            ],
            "debuffType": "HELPFUL",
            "event": "Health",
            "matchesShowOn": "showAlways",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10
      },
      "uid": "P97S9qdems0",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": -2.2222222222222,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r)  \nend\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\n\n\naura_env.clickableFrame:SetScript(\"OnClick\", function()\n        SendChatMessage(\"Please buff Fortitude\", \"RAID\")\n    end\n)",
          "do_custom": true
        },
        "start": []
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Raid Buffs",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": true,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "buffed"
          }
        },
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                1,
                0.64705882352941,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "op": "<",
                "trigger": 1,
                "value": "300",
                "variable": "expirationTime"
              },
              {
                "op": ">",
                "trigger": 1,
                "value": 1,
                "variable": "buffed"
              }
            ],
            "op": "<",
            "trigger": -2,
            "variable": "AND"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 135941,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": -1,
      "id": "Light 3",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": true,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Buffs: Group - Mage",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Blessing of Light",
          "text_text_format_n_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%p",
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [],
            "auraspellids": [
              "25890"
            ],
            "debuffType": "HELPFUL",
            "event": "Health",
            "matchesShowOn": "showAlways",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10
      },
      "uid": "izoij3bSkcQ",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": -2.2222222222222,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r)  \nend\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\n\n\naura_env.clickableFrame:SetScript(\"OnClick\", function()\n        SendChatMessage(\"Please buff Fortitude\", \"RAID\")\n    end\n)",
          "do_custom": true
        },
        "start": []
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Raid Buffs",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": true,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "buffed"
          }
        },
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                1,
                0.64705882352941,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "op": "<",
                "trigger": 1,
                "value": "300",
                "variable": "expirationTime"
              },
              {
                "op": ">",
                "trigger": 1,
                "value": 1,
                "variable": "buffed"
              }
            ],
            "op": "<",
            "trigger": -2,
            "variable": "AND"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 135941,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": -1,
      "id": "Spirit 2",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": true,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Buffs: Group - Mage",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "Prayer of Spirit",
          "text_text_format_n_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%p",
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [],
            "auraspellids": [
              "27681"
            ],
            "debuffType": "HELPFUL",
            "event": "Health",
            "matchesShowOn": "showAlways",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10
      },
      "uid": "ucsOINKPmYy",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": -2.2222222222222,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r)  \nend\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\n\n\naura_env.clickableFrame:SetScript(\"OnClick\", function()\n        SendChatMessage(\"Please buff Mark of the Wild\", \"RAID\")\n    end\n)",
          "do_custom": true
        },
        "start": []
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Raid Buffs",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": true,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0,
                1
              ]
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "buffed"
          }
        },
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                1,
                0.64705882352941,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "op": "<",
                "trigger": 1,
                "value": "300",
                "variable": "expirationTime"
              },
              {
                "op": ">",
                "trigger": 1,
                "value": 1,
                "variable": "buffed"
              }
            ],
            "op": "<",
            "trigger": -2,
            "variable": "AND"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "desaturate": false,
      "displayIcon": 136078,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": -1,
      "id": "Gift of the Wild",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": true,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Buffs: Group - Mage",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%n",
          "text_text_format_n_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%p",
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": true,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [],
            "auraspellids": [
              "48470",
              "48469",
              "21850",
              "9884",
              "5234"
            ],
            "debuffType": "HELPFUL",
            "event": "Health",
            "matchesShowOn": "showAlways",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10
      },
      "uid": "CBBGGF8RGls",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": -2.2222222222222,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\n\n\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/cast [nomod, @player] Dalaran Intellect\n/cast [nomod, @player] Arcane Intellect\n/cast [mod, @player] Arcane Brilliance\n/cast [mod, @player] Dalaran Brilliance\n]])",
          "do_custom": true
        },
        "start": []
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Raid Buffs",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": true,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0,
                1
              ]
            },
            {
              "property": "sub.3.text_visible"
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "buffed"
          }
        },
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                1,
                0.64705882352941,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "op": "<",
                "trigger": 1,
                "value": "300",
                "variable": "expirationTime"
              }
            ],
            "op": "<",
            "trigger": 1,
            "value": "300",
            "variable": "expirationTime"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "customText": "function()\n    return %1.n\nend",
      "desaturate": false,
      "displayIcon": 135869,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 1,
      "id": "Arcane Intellect",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": true,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Buffs: Group - Mage",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%1.n",
          "text_text_format_1.n_format": "none",
          "text_text_format_n_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%2.p",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": true,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%1.p",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": true,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [],
            "auraspellids": [
              "43002",
              "42995",
              "61024",
              "23028",
              "10156"
            ],
            "debuffType": "HELPFUL",
            "event": "Health",
            "matchesShowOn": "showAlways",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "s9ruENzR4Ae",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": -2.2222222222222,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": {
          "custom": "if not aura_env.clickableFrame then\n    local r = aura_env.region\n    aura_env.clickableFrame = CreateFrame(\"Button\", \"ConsumeButton\", r, \"SecureActionButtonTemplate\")  \nend\n\naura_env.clickableFrame:SetAllPoints()\naura_env.clickableFrame:SetPoint(\"RIGHT\",150,0)\naura_env.clickableFrame:SetAttribute(\"type\", \"macro\")\n\n\naura_env.clickableFrame:SetAttribute(\"macrotext\", [[\n/cast [nomod, @player] Dalaran Intellect\n/cast [nomod, @player] Arcane Intellect\n/cast [mod, @player] Arcane Brilliance\n/cast [mod, @player] Dalaran Brilliance\n]])",
          "do_custom": true
        },
        "start": []
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Raid Buffs",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "LEFT",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": true,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                0,
                1,
                0,
                1
              ]
            },
            {
              "property": "sub.3.text_visible"
            }
          ],
          "check": {
            "trigger": 1,
            "value": 1,
            "variable": "buffed"
          }
        },
        {
          "changes": [
            {
              "property": "sub.2.text_color",
              "value": [
                1,
                0.64705882352941,
                0,
                1
              ]
            }
          ],
          "check": {
            "checks": [
              {
                "op": "<",
                "trigger": 1,
                "value": "300",
                "variable": "expirationTime"
              }
            ],
            "op": "<",
            "trigger": 1,
            "value": "300",
            "variable": "expirationTime"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": true,
      "customAnchor": "",
      "customText": "function()\n    return %1.n\nend",
      "desaturate": false,
      "displayIcon": 135869,
      "frameStrata": 4,
      "height": 14,
      "icon": true,
      "iconSource": 1,
      "id": "Mage Armor",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_ingroup": true,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Buffs: Group - Mage",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_RIGHT",
          "text_anchorXOffset": 4,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            0,
            0,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%1.n",
          "text_text_format_1.n_format": "none",
          "text_text_format_n_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%2.p",
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_legacy_floor": true,
          "text_text_format_2.p_time_mod_rate": true,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "OUTER_LEFT",
          "text_anchorXOffset": 190,
          "text_anchorYOffset": 0,
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 12,
          "text_fontType": "OUTLINE",
          "text_justify": "LEFT",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%1.p",
          "text_text_format_1.p_format": "timed",
          "text_text_format_1.p_time_dynamic_threshold": 60,
          "text_text_format_1.p_time_format": 0,
          "text_text_format_1.p_time_legacy_floor": true,
          "text_text_format_1.p_time_mod_rate": true,
          "text_text_format_1.p_time_precision": 1,
          "text_text_format_2.p_format": "timed",
          "text_text_format_2.p_time_dynamic_threshold": 60,
          "text_text_format_2.p_time_format": 0,
          "text_text_format_2.p_time_precision": 1,
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 0,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_precision": 1,
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [],
            "auraspellids": [
              "22783"
            ],
            "debuffType": "HELPFUL",
            "event": "Health",
            "matchesShowOn": "showAlways",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "any"
      },
      "uid": "LvwkEpt2fkQ",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 14,
      "xOffset": 0,
      "yOffset": -2.2222222222222,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "alpha": 1,
      "anchorFrameType": "SCREEN",
      "anchorPoint": "CENTER",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [],
      "backdropColor": [
        1,
        1,
        1,
        0.5
      ],
      "border": false,
      "borderBackdrop": "Blizzard Tooltip",
      "borderColor": [
        0,
        0,
        0,
        1
      ],
      "borderEdge": "Square Full White",
      "borderInset": 1,
      "borderOffset": 4,
      "borderSize": 2,
      "conditions": [],
      "config": [],
      "controlledChildren": [
        "Header: Extra Background",
        "Header: Extra",
        "Extra-Group",
        "New 3"
      ],
      "frameStrata": 1,
      "groupIcon": 133710,
      "id": "Extra",
      "information": {
        "forceEvents": true
      },
      "internalVersion": 79,
      "load": {
        "class": {
          "multi": []
        },
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        }
      },
      "parent": "Mage Buff & Consumes",
      "regionType": "group",
      "scale": 1,
      "selfPoint": "CENTER",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [],
      "tocversion": 11505,
      "triggers": [
        {
          "trigger": {
            "debuffType": "HELPFUL",
            "event": "Health",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player"
          },
          "untrigger": []
        }
      ],
      "uid": "dn9IM)6eAFO",
      "url": "https://wago.io/rGIX20sGW/3",
      "version": 3,
      "wagoID": "rGIX20sGW",
      "xOffset": 0,
      "yOffset": 0
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "alpha": 0.8,
      "anchorFrameFrame": "WeakAuras:Header: Extra",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "CENTER",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "blendMode": "BLEND",
      "color": [
        0.054901960784314,
        0.054901960784314,
        0.054901960784314,
        0.95000000298023
      ],
      "conditions": [],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "customAnchor": "",
      "desaturate": false,
      "discrete_rotation": 0,
      "frameStrata": 4,
      "height": 19,
      "id": "Header: Extra Background",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "mirror": false,
      "parent": "Extra",
      "regionType": "texture",
      "rotate": true,
      "rotation": 0,
      "selfPoint": "CENTER",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "border_color": [
            0,
            0,
            0,
            1
          ],
          "border_edge": "Square Full White",
          "border_offset": 0,
          "border_size": 1,
          "border_visible": true,
          "type": "subborder"
        }
      ],
      "texture": "Interface\\AddOns\\WeakAuras\\Media\\Textures\\Square_FullWhite",
      "textureWrapMode": "CLAMP",
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Conditions",
            "names": [],
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "unit",
            "unevent": "auto",
            "unit": "player",
            "use_alwaystrue": true,
            "use_spellName": true,
            "use_unit": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10
      },
      "uid": "PsPLU2MbDlh",
      "url": "https://wago.io/rGIX20sGW/3",
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 200,
      "xOffset": 0,
      "yOffset": -0.11111111111111
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "anchorFrameFrame": "WeakAuras:Tracker Background",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "TOP",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "automaticWidth": "Fixed",
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "yOffsetRelative",
              "value": -14
            }
          ],
          "check": {
            "op": "ACTIVE_TALENT_GROUP_CHANGED",
            "trigger": -1,
            "value": "function()\n    local _, _, classIndex = UnitClass(\"player\");\n    -- Paladin\n    if(classIndex == 2) then \n        -- Beacon of Light (Holy Spec)\n        local _, _, _, _, beaconSlct, _, _, _ = GetTalentInfo(1, 23, false);    \n        if(beaconSlct == 1) then\n            return true            \n        else\n            return false\n        end\n    elseif (classIndex == 3) then -- Hunter\n        return true\n    elseif (classIndex == 8) then -- Mage\n        return true\n    elseif (classIndex == 9) then -- Warlock\n        return true\n    elseif (classIndex == 11) then -- Druid\n        local name, _, _, _, boomkinSpec, _, _, _ = GetTalentInfo(1, 23, false);\n        if(specSelect == 0) then\n            return true            \n        else\n            return false\n        end\n    else\n        return false\n    end\nend",
            "variable": "customcheck"
          }
        },
        {
          "changes": [
            {
              "property": "yOffsetRelative",
              "value": -40
            }
          ],
          "check": {
            "op": "ACTIVE_TALENT_GROUP_CHANGED",
            "trigger": -1,
            "value": "function()\n    local _, _, classIndex = UnitClass(\"player\");\n    \n    -- Paladin\n    if(classIndex == 2) then \n        local _, _, _, _, protPala, _, _, _ = GetTalentInfo(2, 23, false);                -- Protection\n        if(protPala == 1) then\n            return true   \n            \n        else\n            return false\n        end\n    else\n        return false\n    end\nend\n\n\n",
            "variable": "customcheck"
          },
          "linked": true
        },
        {
          "changes": [
            {
              "property": "yOffsetRelative",
              "value": -28
            }
          ],
          "check": {
            "op": "ACTIVE_TALENT_GROUP_CHANGED",
            "trigger": -1,
            "value": "function()\n    local _, _, classIndex = UnitClass(\"player\");\n    \n    -- Priest\n    if(classIndex == 5) then \n        local _, _, _, _, shadowPriest, _, _, _ = GetTalentInfo(3, 18, false);                -- Shadow\n        if(shadowPriest == 1) then\n            return true   \n            \n        else\n            return false\n        end\n    else\n        return false\n    end\nend\n\n\n",
            "variable": "customcheck"
          },
          "linked": true
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "customAnchor": "",
      "customTextUpdate": "update",
      "displayText": "World Buffs",
      "fixedWidth": 200,
      "font": "Gilroy Bold",
      "fontSize": 12,
      "frameStrata": 4,
      "id": "Header: Extra",
      "information": {
        "forceEvents": true,
        "ignoreOptionsEventErrors": true
      },
      "internalVersion": 79,
      "justify": "CENTER",
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true,
            "WARLOCK": true
          },
          "single": "MAGE"
        },
        "faction": {
          "multi": {
            "Alliance": true
          },
          "single": "Alliance"
        },
        "ingroup": {
          "multi": {
            "raid": true
          },
          "single": "raid"
        },
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "outline": "OUTLINE",
      "parent": "Extra",
      "regionType": "text",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "shadowColor": [
        0,
        0,
        0,
        1
      ],
      "shadowXOffset": 1,
      "shadowYOffset": -1,
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Conditions",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "unit",
            "unevent": "auto",
            "unit": "player",
            "use_alwaystrue": true,
            "use_unit": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10
      },
      "uid": "c5FU3FMdAJ5",
      "url": "https://wago.io/rGIX20sGW/3",
      "version": 3,
      "wagoID": "rGIX20sGW",
      "wordWrap": "WordWrap",
      "xOffset": 0,
      "yOffset": -340.9104416687
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "align": "CENTER",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Extra Background",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "CENTER",
      "animate": false,
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "arcLength": 360,
      "authorOptions": [],
      "backdropColor": [
        1,
        1,
        1,
        0.5
      ],
      "border": false,
      "borderBackdrop": "Blizzard Tooltip",
      "borderColor": [
        0,
        0,
        0,
        1
      ],
      "borderEdge": "Square Full White",
      "borderInset": 1,
      "borderOffset": 4,
      "borderSize": 2,
      "centerType": "LR",
      "columnSpace": 1,
      "conditions": [],
      "config": [],
      "constantFactor": "RADIUS",
      "controlledChildren": [
        "DMF",
        "Ony",
        "Songflower"
      ],
      "frameStrata": 1,
      "fullCircle": true,
      "gridType": "RD",
      "gridWidth": 5,
      "groupIcon": 133709,
      "grow": "HORIZONTAL",
      "id": "Extra-Group",
      "information": {
        "forceEvents": true
      },
      "internalVersion": 79,
      "limit": 5,
      "load": {
        "class": {
          "multi": []
        },
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        }
      },
      "parent": "Extra",
      "radius": 200,
      "regionType": "dynamicgroup",
      "rotation": 0,
      "rowSpace": 1,
      "scale": 1,
      "selfPoint": "CENTER",
      "semver": "1.0.2",
      "sort": "none",
      "sortHybridTable": {
        "DMF": false,
        "Fervor": false,
        "Songflower": false
      },
      "source": "import",
      "space": 20,
      "stagger": 0,
      "stepAngle": 15,
      "subRegions": [],
      "tocversion": 11505,
      "triggers": [
        {
          "trigger": {
            "debuffType": "HELPFUL",
            "event": "Health",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player"
          },
          "untrigger": []
        }
      ],
      "uid": "ZJzrkdscU)D",
      "url": "https://wago.io/rGIX20sGW/3",
      "useLimit": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "xOffset": 0,
      "yOffset": -35
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Extra Background",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "CENTER",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": true,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "desaturate",
              "value": true
            }
          ],
          "check": {
            "trigger": 1,
            "value": 0,
            "variable": "buffed"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": false,
      "customAnchor": "",
      "desaturate": false,
      "frameStrata": 4,
      "height": 32,
      "icon": true,
      "iconSource": -1,
      "id": "DMF",
      "information": {
        "forceEvents": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": true,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "HUNTER": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true
          },
          "single": "MAGE"
        },
        "faction": [],
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Extra-Group",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "CENTER",
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 16,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%p",
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 60,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": false,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "glow": false,
          "glowBorder": false,
          "glowColor": [
            1,
            1,
            1,
            1
          ],
          "glowDuration": 1,
          "glowFrequency": 0.25,
          "glowLength": 10,
          "glowLines": 8,
          "glowScale": 1,
          "glowThickness": 1,
          "glowType": "buttonOverlay",
          "glowXOffset": 0,
          "glowYOffset": 0,
          "type": "subglow",
          "useGlowColor": false
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auraspellids": [
              "23768"
            ],
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "itemName": 4378,
            "matchesShowOn": "showAlways",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unevent": "auto",
            "unit": "player",
            "useExactSpellId": true,
            "useName": false,
            "use_exact_itemName": true,
            "use_itemName": true,
            "use_unit": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "customTriggerLogic": "function(t)\n    return t[1] and not aura_env.config.Inject_Potion\nend",
        "disjunctive": "any"
      },
      "uid": "iEhSeolRu0T",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 32,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Extra Background",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "CENTER",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": true,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "desaturate",
              "value": true
            }
          ],
          "check": {
            "trigger": 1,
            "value": 0,
            "variable": "buffed"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": false,
      "customAnchor": "",
      "desaturate": false,
      "frameStrata": 4,
      "height": 32,
      "icon": true,
      "iconSource": -1,
      "id": "Ony",
      "information": {
        "forceEvents": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": true,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "HUNTER": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true
          },
          "single": "MAGE"
        },
        "faction": [],
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Extra-Group",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "CENTER",
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 16,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%p",
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 60,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": false,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "glow": false,
          "glowBorder": false,
          "glowColor": [
            1,
            1,
            1,
            1
          ],
          "glowDuration": 1,
          "glowFrequency": 0.25,
          "glowLength": 10,
          "glowLines": 8,
          "glowScale": 1,
          "glowThickness": 1,
          "glowType": "buttonOverlay",
          "glowXOffset": 0,
          "glowYOffset": 0,
          "type": "subglow",
          "useGlowColor": false
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auraspellids": [
              "355363"
            ],
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "itemName": 4378,
            "matchesShowOn": "showAlways",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unevent": "auto",
            "unit": "player",
            "useExactSpellId": true,
            "useName": false,
            "use_exact_itemName": true,
            "use_itemName": true,
            "use_unit": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "customTriggerLogic": "function(t)\n    return t[1] and not aura_env.config.Inject_Potion\nend",
        "disjunctive": "any"
      },
      "uid": "MmN3wBCAQLv",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 32,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Extra Background",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "CENTER",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [
        {
          "noMerge": false,
          "text": "Buffs and Consumables v3.6",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "fontSize": "medium",
          "text": "Tracks consumables and buffs.\nClickable consumables and class specific buffs.\n\nWeakaura shows by opening character panel (Default keybind \"C\")\n",
          "type": "description",
          "width": 1.5
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.25
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 0.6
        },
        {
          "fontSize": "medium",
          "text": "\n- By|cFF3FC7EB Highmore|r, edited b |cffAAD372 Shirati",
          "type": "description",
          "width": 1
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "height": 1,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "noMerge": false,
          "text": "Anchor Point",
          "type": "header",
          "useName": true,
          "width": 1
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": true,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Untick this option to freemove anchor point.\nMove WA called |cFFFF0000CornerPosition|r found in  |T132996:0|t Config",
          "type": "description",
          "width": 1.2
        },
        {
          "default": true,
          "desc": "Toggle Free/Paper Doll Anchor",
          "key": "paper_doll_anchor",
          "name": "Anchor to Paper Doll Frame",
          "type": "toggle",
          "useDesc": true,
          "width": 0.8
        },
        {
          "height": 2,
          "type": "space",
          "useHeight": false,
          "variableWidth": true,
          "width": 2
        },
        {
          "fontSize": "medium",
          "text": "Additional Character Stat Addons",
          "type": "description",
          "width": 1.2
        },
        {
          "default": 1,
          "desc": "Character Frame Addon",
          "key": "StatsAnchor",
          "name": "Character Frame Addon",
          "type": "select",
          "useDesc": true,
          "values": [
            "Default WoW (None)",
            "Extended Character Stats",
            "|cFF3FC7EBWrath|rArmory",
            "GearQuipper"
          ],
          "width": 0.8
        }
      ],
      "auto": true,
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [
        {
          "changes": [
            {
              "property": "desaturate",
              "value": true
            }
          ],
          "check": {
            "trigger": 1,
            "value": 0,
            "variable": "buffed"
          }
        }
      ],
      "config": {
        "StatsAnchor": 1,
        "paper_doll_anchor": true
      },
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": false,
      "customAnchor": "",
      "desaturate": false,
      "frameStrata": 4,
      "height": 32,
      "icon": true,
      "iconSource": -1,
      "id": "Songflower",
      "information": {
        "forceEvents": true
      },
      "internalVersion": 79,
      "inverse": false,
      "keepAspectRatio": true,
      "load": {
        "class": {
          "multi": {
            "DRUID": true,
            "HUNTER": true,
            "MAGE": true,
            "PALADIN": true,
            "PRIEST": true,
            "SHAMAN": true
          },
          "single": "MAGE"
        },
        "faction": [],
        "level": [
          "60"
        ],
        "level_operator": [
          ">="
        ],
        "namerealm": "Highmore",
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_class": true,
        "use_level": false,
        "use_namerealm": false,
        "use_never": false,
        "zoneIds": ""
      },
      "parent": "Extra-Group",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "TOP",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "anchorXOffset": 0,
          "anchorYOffset": 0,
          "rotateText": "NONE",
          "text_anchorPoint": "CENTER",
          "text_automaticWidth": "Auto",
          "text_color": [
            1,
            1,
            1,
            1
          ],
          "text_fixedWidth": 64,
          "text_font": "Gilroy Bold",
          "text_fontSize": 16,
          "text_fontType": "OUTLINE",
          "text_justify": "CENTER",
          "text_selfPoint": "AUTO",
          "text_shadowColor": [
            0,
            0,
            0,
            1
          ],
          "text_shadowXOffset": 0,
          "text_shadowYOffset": 0,
          "text_text": "%p",
          "text_text_format_p_format": "timed",
          "text_text_format_p_time_dynamic_threshold": 60,
          "text_text_format_p_time_format": 0,
          "text_text_format_p_time_legacy_floor": false,
          "text_text_format_p_time_mod_rate": true,
          "text_text_format_p_time_precision": 1,
          "text_text_format_s_format": "none",
          "text_visible": true,
          "text_wordWrap": "WordWrap",
          "type": "subtext"
        },
        {
          "glow": false,
          "glowBorder": false,
          "glowColor": [
            1,
            1,
            1,
            1
          ],
          "glowDuration": 1,
          "glowFrequency": 0.25,
          "glowLength": 10,
          "glowLines": 8,
          "glowScale": 1,
          "glowThickness": 1,
          "glowType": "buttonOverlay",
          "glowXOffset": 0,
          "glowYOffset": 0,
          "type": "subglow",
          "useGlowColor": false
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auraspellids": [
              "15366"
            ],
            "debuffType": "HELPFUL",
            "duration": "1",
            "event": "Item Count",
            "itemName": 4378,
            "matchesShowOn": "showAlways",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unevent": "auto",
            "unit": "player",
            "useExactSpellId": true,
            "useName": false,
            "use_exact_itemName": true,
            "use_itemName": true,
            "use_unit": true
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "customTriggerLogic": "function(t)\n    return t[1] and not aura_env.config.Inject_Potion\nend",
        "disjunctive": "any"
      },
      "uid": "vRHBKn9dXCl",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 32,
      "xOffset": 0,
      "yOffset": 0,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "alpha": 1,
      "anchorFrameType": "SCREEN",
      "anchorPoint": "CENTER",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [],
      "backdropColor": [
        1,
        1,
        1,
        0.5
      ],
      "border": false,
      "borderBackdrop": "Blizzard Tooltip",
      "borderColor": [
        0,
        0,
        0,
        1
      ],
      "borderEdge": "Square Full White",
      "borderInset": 1,
      "borderOffset": 4,
      "borderSize": 2,
      "conditions": [],
      "config": [],
      "controlledChildren": [
        "Chronoboon Display - Fervor",
        "Chronoboon Display - Ony",
        "Chronoboon Display - DMF",
        "Chronoboon Display - SF"
      ],
      "frameStrata": 1,
      "groupIcon": 133881,
      "id": "New 3",
      "information": [],
      "internalVersion": 79,
      "load": {
        "class": {
          "multi": []
        },
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        }
      },
      "parent": "Extra",
      "regionType": "group",
      "scale": 1,
      "selfPoint": "CENTER",
      "semver": "1.0.2",
      "source": "import",
      "subRegions": [],
      "tocversion": 11505,
      "triggers": [
        {
          "trigger": {
            "debuffType": "HELPFUL",
            "event": "Health",
            "names": [],
            "spellIds": [],
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player"
          },
          "untrigger": []
        }
      ],
      "uid": "tN((JXwQa79",
      "url": "https://wago.io/rGIX20sGW/3",
      "version": 3,
      "wagoID": "rGIX20sGW",
      "xOffset": 0,
      "yOffset": 0
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Extra Background",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "CENTER",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [],
      "automaticWidth": "Auto",
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [],
      "config": [],
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": false,
      "customText": "function()\n    local display = nil\n    local name = GetSpellInfo(349981)\n    local index = nil;\n    for i=1,40 do\n        local buff = UnitBuff(\"player\", i)\n        if buff == name then\n            index = i\n            break\n        end\n    end\n    if name and index then\n        local inline = select(1, WeakAuras.GetAuraTooltipInfo(\"player\",index))\n        inline = string.gsub(inline,\"World effects suspended:\",\"\")\n        display = inline\n    end\n    return display\nend\n\n\n",
      "customTextUpdate": "event",
      "desaturate": false,
      "displayText": "%n : \n%c\n\n",
      "displayText_format_c_format": "none",
      "displayText_format_n_format": "none",
      "displayText_format_p_format": "timed",
      "displayText_format_p_time_dynamic_threshold": 60,
      "displayText_format_p_time_format": 0,
      "displayText_format_p_time_precision": 1,
      "displayText_format_tooltip1_format": "none",
      "displayText_format_tooltip2_format": "none",
      "displayText_format_tooltip_format": "none",
      "fixedWidth": 200,
      "font": "Expressway",
      "fontSize": 13,
      "frameStrata": 1,
      "height": 16,
      "icon": true,
      "iconSource": -1,
      "id": "Chronoboon Display - Fervor",
      "information": {
        "forceEvents": true
      },
      "internalVersion": 79,
      "inverse": false,
      "justify": "LEFT",
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": []
        },
        "level": [
          "60"
        ],
        "level_operator": [
          "<="
        ],
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_combat": false,
        "use_level": false,
        "use_namerealm": false
      },
      "outline": "OUTLINE",
      "parent": "New 3",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "BOTTOM",
      "semver": "1.0.2",
      "shadowColor": [
        0,
        0,
        0,
        1
      ],
      "shadowXOffset": 1,
      "shadowYOffset": -1,
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "border_color": [
            1,
            0.93725496530533,
            0,
            1
          ],
          "border_edge": "Square Full White",
          "border_offset": 0,
          "border_size": 1,
          "border_visible": true,
          "type": "subborder"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [
              ""
            ],
            "auraspellids": [
              "349981"
            ],
            "debuffType": "HELPFUL",
            "event": "Cooldown Progress (Spell)",
            "fetchTooltip": true,
            "genericShowOn": "showOnCooldown",
            "names": [],
            "ownOnly": true,
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true,
            "useName": false,
            "use_debuffClass": false,
            "use_genericShowOn": true,
            "use_spellName": true,
            "use_tooltipValue": false,
            "use_track": true,
            "use_unit": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "check": "event",
            "custom": "function()\n    local display = nil\n    local name = GetSpellInfo(349981)\n    local index = nil;\n    for i=1,40 do\n        local buff = UnitBuff(\"player\", i)\n        if buff == name then\n            index = i\n            break\n        end\n    end\n    if name and index then\n        local inline = select(1, WeakAuras.GetAuraTooltipInfo(\"player\",index))\n        inline = string.gsub(inline,\"World effects suspended:\",\"\")\n        display = inline\n        if display:find(\"Fervor\") then \n            return true\n        end\n    end\nend\n\n\n",
            "custom_hide": "timed",
            "custom_type": "status",
            "debuffType": "HELPFUL",
            "events": "SPELL_AURA_APPLIED",
            "type": "custom",
            "unit": "player"
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "all"
      },
      "uid": "2jOAcFVsBGs",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 16,
      "wordWrap": "WordWrap",
      "xOffset": 13,
      "yOffset": -55.645113886848,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Extra Background",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "CENTER",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [],
      "automaticWidth": "Auto",
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [],
      "config": [],
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": false,
      "customText": "function()\n    local display = nil\n    local name = GetSpellInfo(349981)\n    local index = nil;\n    for i=1,40 do\n        local buff = UnitBuff(\"player\", i)\n        if buff == name then\n            index = i\n            break\n        end\n    end\n    if name and index then\n        local inline = select(1, WeakAuras.GetAuraTooltipInfo(\"player\",index))\n        inline = string.gsub(inline,\"World effects suspended:\",\"\")\n        display = inline\n    end\n    return display\nend\n\n\n",
      "customTextUpdate": "event",
      "desaturate": false,
      "displayText": "%n : \n%c\n\n",
      "displayText_format_c_format": "none",
      "displayText_format_n_format": "none",
      "displayText_format_p_format": "timed",
      "displayText_format_p_time_dynamic_threshold": 60,
      "displayText_format_p_time_format": 0,
      "displayText_format_p_time_precision": 1,
      "displayText_format_tooltip1_format": "none",
      "displayText_format_tooltip2_format": "none",
      "displayText_format_tooltip_format": "none",
      "fixedWidth": 200,
      "font": "Expressway",
      "fontSize": 13,
      "frameStrata": 1,
      "height": 16,
      "icon": true,
      "iconSource": -1,
      "id": "Chronoboon Display - Ony",
      "information": {
        "forceEvents": true
      },
      "internalVersion": 79,
      "inverse": false,
      "justify": "LEFT",
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": []
        },
        "level": [
          "60"
        ],
        "level_operator": [
          "<="
        ],
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_combat": false,
        "use_level": false,
        "use_namerealm": false
      },
      "outline": "OUTLINE",
      "parent": "New 3",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "BOTTOM",
      "semver": "1.0.2",
      "shadowColor": [
        0,
        0,
        0,
        1
      ],
      "shadowXOffset": 1,
      "shadowYOffset": -1,
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "border_color": [
            1,
            0.93725496530533,
            0,
            1
          ],
          "border_edge": "Square Full White",
          "border_offset": 0,
          "border_size": 1,
          "border_visible": true,
          "type": "subborder"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [
              ""
            ],
            "auraspellids": [
              "349981"
            ],
            "debuffType": "HELPFUL",
            "event": "Cooldown Progress (Spell)",
            "fetchTooltip": true,
            "genericShowOn": "showOnCooldown",
            "names": [],
            "ownOnly": true,
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true,
            "useName": false,
            "use_debuffClass": false,
            "use_genericShowOn": true,
            "use_spellName": true,
            "use_tooltipValue": false,
            "use_track": true,
            "use_unit": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "check": "event",
            "custom": "function()\n    local display = nil\n    local name = GetSpellInfo(349981)\n    local index = nil;\n    for i=1,40 do\n        local buff = UnitBuff(\"player\", i)\n        if buff == name then\n            index = i\n            break\n        end\n    end\n    if name and index then\n        local inline = select(1, WeakAuras.GetAuraTooltipInfo(\"player\",index))\n        inline = string.gsub(inline,\"World effects suspended:\",\"\")\n        display = inline\n        if display:find(\"Rallying Cry of the Dragonslayer\") then \n            return true\n        end\n    end\nend\n\n\n",
            "custom_hide": "timed",
            "custom_type": "status",
            "debuffType": "HELPFUL",
            "events": "SPELL_AURA_APPLIED",
            "type": "custom",
            "unit": "player"
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "all"
      },
      "uid": "K6S0U28yETS",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 16,
      "wordWrap": "WordWrap",
      "xOffset": 13,
      "yOffset": -55.645113886848,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Extra Background",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "CENTER",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [],
      "automaticWidth": "Auto",
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [],
      "config": [],
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": false,
      "customText": "function()\n    local display = nil\n    local name = GetSpellInfo(349981)\n    local index = nil;\n    for i=1,40 do\n        local buff = UnitBuff(\"player\", i)\n        if buff == name then\n            index = i\n            break\n        end\n    end\n    if name and index then\n        local inline = select(1, WeakAuras.GetAuraTooltipInfo(\"player\",index))\n        inline = string.gsub(inline,\"World effects suspended:\",\"\")\n        display = inline\n    end\n    return display\nend\n\n\n",
      "customTextUpdate": "event",
      "desaturate": false,
      "displayText": "%n : \n%c\n\n",
      "displayText_format_c_format": "none",
      "displayText_format_n_format": "none",
      "displayText_format_p_format": "timed",
      "displayText_format_p_time_dynamic_threshold": 60,
      "displayText_format_p_time_format": 0,
      "displayText_format_p_time_precision": 1,
      "displayText_format_tooltip1_format": "none",
      "displayText_format_tooltip2_format": "none",
      "displayText_format_tooltip_format": "none",
      "fixedWidth": 200,
      "font": "Expressway",
      "fontSize": 13,
      "frameStrata": 1,
      "height": 16,
      "icon": true,
      "iconSource": -1,
      "id": "Chronoboon Display - DMF",
      "information": {
        "forceEvents": true
      },
      "internalVersion": 79,
      "inverse": false,
      "justify": "LEFT",
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": []
        },
        "level": [
          "60"
        ],
        "level_operator": [
          "<="
        ],
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_combat": false,
        "use_level": false,
        "use_namerealm": false
      },
      "outline": "OUTLINE",
      "parent": "New 3",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "BOTTOM",
      "semver": "1.0.2",
      "shadowColor": [
        0,
        0,
        0,
        1
      ],
      "shadowXOffset": 1,
      "shadowYOffset": -1,
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "border_color": [
            1,
            0.93725496530533,
            0,
            1
          ],
          "border_edge": "Square Full White",
          "border_offset": 0,
          "border_size": 1,
          "border_visible": true,
          "type": "subborder"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [
              ""
            ],
            "auraspellids": [
              "349981"
            ],
            "debuffType": "HELPFUL",
            "event": "Cooldown Progress (Spell)",
            "fetchTooltip": true,
            "genericShowOn": "showOnCooldown",
            "names": [],
            "ownOnly": true,
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true,
            "useName": false,
            "use_debuffClass": false,
            "use_genericShowOn": true,
            "use_spellName": true,
            "use_tooltipValue": false,
            "use_track": true,
            "use_unit": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "check": "event",
            "custom": "function()\n    local display = nil\n    local name = GetSpellInfo(349981)\n    local index = nil;\n    for i=1,40 do\n        local buff = UnitBuff(\"player\", i)\n        if buff == name then\n            index = i\n            break\n        end\n    end\n    if name and index then\n        local inline = select(1, WeakAuras.GetAuraTooltipInfo(\"player\",index))\n        inline = string.gsub(inline,\"World effects suspended:\",\"\")\n        display = inline\n        if display:find(\"Sayge\") then \n            return true\n        end\n    end\nend\n\n\n",
            "custom_hide": "timed",
            "custom_type": "status",
            "debuffType": "HELPFUL",
            "events": "SPELL_AURA_APPLIED",
            "type": "custom",
            "unit": "player"
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "all"
      },
      "uid": "WURDW3DeMB3",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 16,
      "wordWrap": "WordWrap",
      "xOffset": -38.763409233093,
      "yOffset": -55.645113886848,
      "zoom": 0
    },
    {
      "actions": {
        "finish": [],
        "init": [],
        "start": []
      },
      "adjustedMax": "",
      "adjustedMin": "",
      "alpha": 1,
      "anchorFrameFrame": "WeakAuras:Header: Extra Background",
      "anchorFrameType": "SELECTFRAME",
      "anchorPoint": "CENTER",
      "animation": {
        "finish": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "main": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        },
        "start": {
          "duration_type": "seconds",
          "easeStrength": 3,
          "easeType": "none",
          "type": "none"
        }
      },
      "authorOptions": [],
      "automaticWidth": "Auto",
      "color": [
        1,
        1,
        1,
        1
      ],
      "conditions": [],
      "config": [],
      "cooldown": false,
      "cooldownEdge": false,
      "cooldownSwipe": true,
      "cooldownTextDisabled": false,
      "customText": "function()\n    local display = nil\n    local name = GetSpellInfo(349981)\n    local index = nil;\n    for i=1,40 do\n        local buff = UnitBuff(\"player\", i)\n        if buff == name then\n            index = i\n            break\n        end\n    end\n    if name and index then\n        local inline = select(1, WeakAuras.GetAuraTooltipInfo(\"player\",index))\n        inline = string.gsub(inline,\"World effects suspended:\",\"\")\n        display = inline\n    end\n    return display\nend\n\n\n",
      "customTextUpdate": "event",
      "desaturate": false,
      "displayText": "%n : \n%c\n\n",
      "displayText_format_c_format": "none",
      "displayText_format_n_format": "none",
      "displayText_format_p_format": "timed",
      "displayText_format_p_time_dynamic_threshold": 60,
      "displayText_format_p_time_format": 0,
      "displayText_format_p_time_precision": 1,
      "displayText_format_tooltip1_format": "none",
      "displayText_format_tooltip2_format": "none",
      "displayText_format_tooltip_format": "none",
      "fixedWidth": 200,
      "font": "Expressway",
      "fontSize": 13,
      "frameStrata": 1,
      "height": 16,
      "icon": true,
      "iconSource": -1,
      "id": "Chronoboon Display - SF",
      "information": {
        "forceEvents": true
      },
      "internalVersion": 79,
      "inverse": false,
      "justify": "LEFT",
      "keepAspectRatio": false,
      "load": {
        "class": {
          "multi": []
        },
        "level": [
          "60"
        ],
        "level_operator": [
          "<="
        ],
        "size": {
          "multi": []
        },
        "spec": {
          "multi": []
        },
        "talent": {
          "multi": []
        },
        "use_combat": false,
        "use_level": false,
        "use_namerealm": false
      },
      "outline": "OUTLINE",
      "parent": "New 3",
      "progressSource": [
        -1,
        ""
      ],
      "regionType": "icon",
      "selfPoint": "BOTTOM",
      "semver": "1.0.2",
      "shadowColor": [
        0,
        0,
        0,
        1
      ],
      "shadowXOffset": 1,
      "shadowYOffset": -1,
      "source": "import",
      "subRegions": [
        {
          "type": "subbackground"
        },
        {
          "border_color": [
            1,
            0.93725496530533,
            0,
            1
          ],
          "border_edge": "Square Full White",
          "border_offset": 0,
          "border_size": 1,
          "border_visible": true,
          "type": "subborder"
        }
      ],
      "tocversion": 11505,
      "triggers": {
        "1": {
          "trigger": {
            "auranames": [
              ""
            ],
            "auraspellids": [
              "349981"
            ],
            "debuffType": "HELPFUL",
            "event": "Cooldown Progress (Spell)",
            "fetchTooltip": true,
            "genericShowOn": "showOnCooldown",
            "names": [],
            "ownOnly": true,
            "realSpellName": 0,
            "spellIds": [],
            "spellName": 0,
            "subeventPrefix": "SPELL",
            "subeventSuffix": "_CAST_START",
            "type": "aura2",
            "unit": "player",
            "useExactSpellId": true,
            "useName": false,
            "use_debuffClass": false,
            "use_genericShowOn": true,
            "use_spellName": true,
            "use_tooltipValue": false,
            "use_track": true,
            "use_unit": true
          },
          "untrigger": []
        },
        "2": {
          "trigger": {
            "check": "event",
            "custom": "function()\n    local display = nil\n    local name = GetSpellInfo(349981)\n    local index = nil;\n    for i=1,40 do\n        local buff = UnitBuff(\"player\", i)\n        if buff == name then\n            index = i\n            break\n        end\n    end\n    if name and index then\n        local inline = select(1, WeakAuras.GetAuraTooltipInfo(\"player\",index))\n        inline = string.gsub(inline,\"World effects suspended:\",\"\")\n        display = inline\n        if display:find(\"Songflower Serenade\") then \n            return true\n        end\n    end\nend\n\n\n",
            "custom_hide": "timed",
            "custom_type": "status",
            "debuffType": "HELPFUL",
            "events": "SPELL_AURA_APPLIED",
            "type": "custom",
            "unit": "player"
          },
          "untrigger": []
        },
        "activeTriggerMode": -10,
        "disjunctive": "all"
      },
      "uid": "HyGsNCQpYoz",
      "url": "https://wago.io/rGIX20sGW/3",
      "useAdjustededMax": false,
      "useAdjustededMin": false,
      "useCooldownModRate": true,
      "useTooltip": false,
      "version": 3,
      "wagoID": "rGIX20sGW",
      "width": 16,
      "wordWrap": "WordWrap",
      "xOffset": 65.343864631653,
      "yOffset": -55.645113886848,
      "zoom": 0
    }
  ],
  "d": {
    "actions": {
      "finish": [],
      "init": [],
      "start": []
    },
    "alpha": 1,
    "anchorFrameFrame": "PaperDollFrame",
    "anchorFrameParent": true,
    "anchorFrameType": "SELECTFRAME",
    "anchorPoint": "TOPLEFT",
    "animation": {
      "finish": {
        "duration_type": "seconds",
        "easeStrength": 3,
        "easeType": "none",
        "type": "none"
      },
      "main": {
        "duration_type": "seconds",
        "easeStrength": 3,
        "easeType": "none",
        "type": "none"
      },
      "start": {
        "duration_type": "seconds",
        "easeStrength": 3,
        "easeType": "none",
        "type": "none"
      }
    },
    "authorOptions": [],
    "backdropColor": [
      1,
      1,
      1,
      0.5
    ],
    "border": false,
    "borderBackdrop": "Blizzard Tooltip",
    "borderColor": [
      0,
      0,
      0,
      1
    ],
    "borderEdge": "Square Full White",
    "borderInset": 1,
    "borderOffset": 4,
    "borderSize": 2,
    "conditions": [],
    "config": [],
    "controlledChildren": [
      "Config",
      "Consumables",
      "Raid Buffs",
      "Extra"
    ],
    "customAnchor": "\n",
    "desc": "Inspired by Highmore/Shirati: https://wago.io/OhXkQ1va_",
    "frameStrata": 1,
    "groupIcon": "133799",
    "id": "Mage Buff & Consumes",
    "information": {
      "forceEvents": true,
      "groupOffset": true,
      "ignoreOptionsEventErrors": true
    },
    "internalVersion": 79,
    "load": {
      "class": {
        "multi": []
      },
      "size": {
        "multi": []
      },
      "spec": {
        "multi": []
      },
      "talent": {
        "multi": []
      },
      "use_class": "false",
      "zoneIds": ""
    },
    "regionType": "group",
    "scale": 1,
    "selfPoint": "BOTTOMLEFT",
    "semver": "1.0.2",
    "source": "import",
    "subRegions": [],
    "tocversion": 11505,
    "triggers": [
      {
        "trigger": {
          "debuffType": "HELPFUL",
          "event": "Health",
          "names": [],
          "spellIds": [],
          "subeventPrefix": "SPELL",
          "subeventSuffix": "_CAST_START",
          "type": "aura2",
          "unit": "player"
        },
        "untrigger": []
      }
    ],
    "uid": "N)hsKUP6CNg",
    "url": "https://wago.io/rGIX20sGW/3",
    "version": 3,
    "wagoID": "rGIX20sGW",
    "xOffset": 243.99999160767,
    "yOffset": -13.333279079861
  },
  "m": "d",
  "s": "5.18.1",
  "v": 2000,
  "wagoID": "rGIX20sGW"
}
