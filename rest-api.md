|         TYPE      |WEB|API|URI|DESCRIPTION|
|------------------ |---|---|---|-----------|
| create & edit     | * | * | /\[users \| teachers \| students\]/${userId}/entities | 实体列表 |
| create & edit     |   | * | /\[users \| teachers \| students\]/${userId}/entities/${entityId} | 实体 |
| create & edit     |   | * | /\[users \| teachers \| students\]/${userId}/entities/${entityId}/checkers | 审批人 |
| public view       | * | * | /entities | 实体列表 |
| public view       | * | * | /entities/${entityId} | 实体 |
| organization view | * | * | /departments/${departmentId}/entities/${entityId} | 部门视图 |
| organization view | * | * | /adminClasses/${adminClassId}/entities/${entityId} | 班级视图 |
| approval process  | * | * | /reviewers/${userId}/entities | 审核列表 |
| approval process  | * |   | /reviewers/${userId}/entities#/${entityId}/workitems/${workitemId} | 待办项 |
| approval process  |   | * | /reviewers/${userId}/entities/${entityId}/workitems/${workitemId} | 数据 |
| approval process  |   | * | /reviewers/${userId}/entities/${entityId}/reviewers?type=\[check \| approve\] | 审核人 |
| setup             | * | * | /settings/entities | 实体列表 |
| setup             |   | * | /settings/entities/${entityId} | 实体 |