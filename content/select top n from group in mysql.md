---
created: 2022-10-17T20:49:44-07:00
updated: 2022-10-17T20:49:44-07:00
---
```
select reference_id, req_file_id  
from (select reference_id, req_file_id, @rn := IF(@prev = req_file_id, @rn + 1, 1) as rn,  
             @prev:=req_file_id  
      from ptech_batch_transaction  
               join (select @prev := NULL, @rn := 0) as vars  
      where req_file_id in ('89f1fe1f-1f4e-44c8-8bb5-e81957c3da31', '3bd511bd-20bb-46de-800f-1d1375bfd834')  
      order by  req_file_id, reference_id) as t1  
where rn <= 2;
```

Pieced together from https://stackoverflow.com/a/12117654/114583