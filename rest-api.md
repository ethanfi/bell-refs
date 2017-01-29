|         TYPE      |WEB|API|URI|DESCRIPTION|
|------------------ |---|---|---|-----------|
| create & edit     | * | * | /\[users|teachers|students\]/${userId}/entities ||
| create & edit     |   | * | /\[users|teachers|students\]/${userId}/entities/${entityId} ||
| public view       | * | * | /entities ||
| public view       | * | * | /entities/${entities} ||
| organization view | * | * | /departments/${departmentId}/entities/${entities} ||
| organization view | * | * | /adminClasses/${adminClassId}/entities/${entities} ||
| approval request  | * | * | /requests/entities | 独立审核视图 |
| approval request  | * |   | /requests/entities#/${entityId}/reviews/${workitemId} | 独立审核视图 |
| approval request  | * | * | /entities/${entityId}/reviews/${workitemId} | 待办事项 |
| approval request  | * | * | /entities/${entityId}/receivers?type=[check|approve] ||
| setup             | * | * | /settings/entities ||
| setup             |   | * | /settings/entities/${entityId} ||