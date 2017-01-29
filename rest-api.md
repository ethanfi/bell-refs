|         TYPE      |WEB|API|URI|DESCRIPTION|
|------------------ |---|---|---|-----------|
| create & edit     | * | * | /\[`users` \| `teachers` \| `students`\]/${userId}/entities ||
| create & edit     |   | * | /\[`users` \| `teachers` \| `students`\]/${userId}/entities/${entityId} ||
| public view       | * | * | /entities ||
| public view       | * | * | /entities/${entityId} ||
| organization view | * | * | /`departments`/${departmentId}/entities/${entityId} ||
| organization view | * | * | /`adminClasses`/${adminClassId}/entities/${entityId} ||
| approval process  | * | * | /`reviewers`/${userId}/entities | 独立审核视图 |
| approval process  | * |   | /`reviewers`/${userId}/entities#/${entityId}/workitems/${workitemId} ||
| approval process  |   | * | /`reviewers`/${userId}/entities/${entityId}/workitems/${workitemId} ||
| approval process  | * | * | /entities/${entityId}/reviewers?type=\[check \| approve\] ||
| setup             | * | * | /`settings`/entities ||
| setup             |   | * | /`settings`/entities/${entityId} ||