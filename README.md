# deploy-and-manage-adk-service

1. Prepare agent dir
2. Create database to be used by session service
3. Configure session service
4. Deploy
5. Load test

Trigger the Locust load test with the following command:

```bash
locust -f load_test.py \
-H http://127.0.0.1:8000 \
--headless \
-t 120s -u 60 -r 5 \
--csv=.results/results \
--html=.results/report.html
```
