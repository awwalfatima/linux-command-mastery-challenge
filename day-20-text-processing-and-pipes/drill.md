#nano drill.log
" 2026-08-31 10:16:05 ERROR Database connection failed
2026-08-31 10:16:05 ERROR Database connection failed
2026-08-31 10:18:12 ERROR Permission denied
2026-08-31 10:18:12 ERROR Permission denied "
#grep "ERROR" drill.log
#grep "ERROR" drill.log | awk '{print $1, $2}'
#grep "ERROR" drill.log | awk '{print $1, $2}' | sort
#grep "ERROR" drill.log | awk '{print $1, $2}' | sort | uniq

