Тестовое задание №1

SELECT 
    task_status.issue_key AS N,
    task_info.name AS name
FROM 
    task_info
RIGHT JOIN task_status ON task_status.issue_key = task_info.issue_key
WHERE 
    task_info.type = 'BUG' AND task_status.status = 'in progress' AND task_status.start_time >= '2021/04/01' AND task.status.start_time <= '2021/04/31'
    
