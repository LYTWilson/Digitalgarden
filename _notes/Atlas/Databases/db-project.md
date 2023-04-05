---

database-plugin: basic

---

```yaml:dbfolder
name: new database
description: new description
columns:
  aliases:
    input: tags
    accessorKey: aliases
    key: aliases
    id: aliases
    label: aliases
    position: 1
    skipPersist: false
    isHidden: true
    sortIndex: -1
    options:
      - { label: "SM", value: "SM", color: "hsl(12, 95%, 90%)"}
      - { label: "LOP", value: "LOP", color: "hsl(252, 95%, 90%)"}
      - { label: "LOP Theory", value: "LOP Theory", color: "hsl(198, 95%, 90%)"}
      - { label: "Remember/know procedure", value: "Remember/know procedure", color: "hsl(199, 95%, 90%)"}
      - { label: "RK procedure", value: "RK procedure", color: "hsl(303, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  database-plugin:
    input: text
    accessorKey: database-plugin
    key: database-plugin
    id: database-plugin
    label: database-plugin
    position: 4
    skipPersist: false
    isHidden: true
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  tag:
    input: tags
    accessorKey: tag
    key: tag
    id: tag
    label: tag
    position: 7
    skipPersist: false
    isHidden: true
    sortIndex: -1
    width: 76
    options:
      - { label: "lecture", value: "lecture", color: "hsl(165, 95%, 90%)"}
      - { label: "seedling", value: "seedling", color: "hsl(290, 95%, 90%)"}
      - { label: "project", value: "project", color: "hsl(70, 95%, 90%)"}
      - { label: "input/video", value: "input/video", color: "hsl(90, 95%, 90%)"}
      - { label: "fern", value: "fern", color: "hsl(139, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  type:
    input: text
    accessorKey: type
    key: type
    id: type
    label: type
    position: 8
    skipPersist: false
    isHidden: true
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  __file__:
    key: __file__
    id: __file__
    input: markdown
    label: File
    accessorKey: __file__
    isMetadata: true
    skipPersist: false
    isDragDisabled: false
    csvCandidate: true
    position: 2
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  __created__:
    key: __created__
    id: __created__
    input: metadata_time
    label: Created
    accessorKey: __created__
    isMetadata: true
    isDragDisabled: false
    skipPersist: false
    csvCandidate: true
    position: 6
    isHidden: false
    sortIndex: -1
    width: 215
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  __tasks__:
    key: __tasks__
    id: __tasks__
    input: task
    label: Task
    accessorKey: __tasks__
    isMetadata: true
    isDragDisabled: false
    skipPersist: false
    csvCandidate: false
    position: 3
    isHidden: false
    sortIndex: -1
    width: 155
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: false
      footer_type: none
      persist_changes: false
  deadline:
    input: text
    accessorKey: deadline
    key: deadline
    id: deadline
    label: deadline
    position: 5
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
config:
  remove_field_when_delete_column: false
  cell_size: normal
  sticky_first_column: false
  group_folder_column: 
  remove_empty_folders: false
  automatically_group_files: true
  hoist_files_with_empty_attributes: true
  show_metadata_created: true
  show_metadata_modified: false
  show_metadata_tasks: true
  show_metadata_inlinks: false
  show_metadata_outlinks: false
  source_data: tag
  source_form_result: "#project"
  source_destination_path: /
  row_templates_folder: /
  current_row_template: 
  pagination_size: 10
  font_size: 16
  enable_js_formulas: false
  formula_folder_path: /
  inline_default: false
  inline_new_position: top
  date_format: yyyy-MM-dd
  datetime_format: "yyyy-MM-dd HH:mm:ss"
  metadata_date_format: "yyyy-MM-dd HH:mm:ss"
  enable_footer: false
  implementation: default
filters:
  enabled: true
  conditions:
      - field: tag
        operator: CONTAINS
        value: "project"
      - field: file.name
        operator: NOT_EQUAL
        value: "tp-School Projects"
```