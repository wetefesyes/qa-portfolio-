
# 1 Сколько всего строк в файле?
## Всего в файле 220000 строк
# 2 Сколько ERROR/WARN/INFO
## ERROR: 30640, WARN: 33318, INFO: 131731
# 3 Последние 20 ERROR
2026-05-26 23:56:39.210 [http-nio-8080-exec-17] ERROR [requestId=2f3dd0d9-b1e1] ru.da.gov.bank.service.AuthService - File not found: /tmp/4c993787-fdb6-f34e-56bd-fc28ef3c6ee9.tmp
2026-05-26 23:56:49.841 [http-nio-8080-exec-3] ERROR [requestId=2c9c65f1-be05] com.zaxxer.hikari.pool.HikariPool - Timeout waiting for response from user-service (5000 ms)
2026-05-26 23:56:50.321 [http-nio-8080-exec-27] ERROR [requestId=e77704cf-22a7] ru.da.gov.bank.security.JwtAuthFilter - Kafka producer timeout after 2922 ms
2026-05-26 23:57:01.750 [http-nio-8080-exec-30] ERROR [requestId=dc40981e-58dc] com.zaxxer.hikari.pool.HikariPool - Transaction rollback: txId=0dc105c7-7ffb-e4c5-d584-5cafb399f8f0, reason=deadlock detected
2026-05-26 23:57:03.078 [http-nio-8080-exec-7] ERROR [requestId=77172782-b001] o.s.web.servlet.DispatcherServlet - Validation failed for field amount: must be greater than 0
2026-05-26 23:57:14.283 [http-nio-8080-exec-6] ERROR [requestId=d326adc3-dbaf] ru.da.gov.bank.service.AuthService - Timeout waiting for response from audit-logger (5000 ms)
2026-05-26 23:57:16.505 [http-nio-8080-exec-21] ERROR [requestId=e64d973b-2e93] ru.da.gov.bank.service.TransferService - Timeout connecting to redis://notification-service:9437
2026-05-26 23:57:26.123 [http-nio-8080-exec-32] ERROR [requestId=a235af44-0246] ru.da.gov.bank.service.AuthService - Failed login attempt: email=grace@bank.test, reason=invalid_credentials
2026-05-26 23:57:29.949 [http-nio-8080-exec-13] ERROR [requestId=8f812417-c238] ru.da.gov.bank.service.AuthService - Hibernate LazyInitializationException: could not initialize proxy
2026-05-26 23:57:37.092 [http-nio-8080-exec-19] ERROR [requestId=63769dac-ff86] ru.da.gov.bank.service.AcquiringService - Timeout waiting for response from webhook-dispatcher (5000 ms)
2026-05-26 23:58:08.303 [http-nio-8080-exec-7] ERROR [requestId=02102edd-c107] org.flywaydb.core.Flyway - Failed login attempt: email=alice@bank.test, reason=invalid_credentials
2026-05-26 23:58:44.141 [http-nio-8080-exec-27] ERROR [requestId=f8eb739a-f8e0] org.flywaydb.core.Flyway - HTTP POST /api/v1/acquiring/charge -> 500 (3297 ms)
2026-05-26 23:58:55.497 [http-nio-8080-exec-6] ERROR [requestId=490898bc-27d4] r.d.g.b.config.RequestLoggingFilter - HTTP POST /api/v1/accounts -> 503 (1068 ms)
2026-05-26 23:58:59.178 [http-nio-8080-exec-3] ERROR [requestId=c761890e-fadc] org.flywaydb.core.Flyway - SQLException: duplicate key value violates unique constraint
2026-05-26 23:59:01.864 [http-nio-8080-exec-19] ERROR [requestId=0eb42da8-59df] ru.da.gov.bank.service.AuthService - Could not commit transaction: lock wait timeout exceeded
2026-05-26 23:59:06.146 [http-nio-8080-exec-3] ERROR [requestId=958c578e-df12] ru.da.gov.bank.service.AuthService - Validation failed for field amount: must be greater than 0
2026-05-26 23:59:24.559 [http-nio-8080-exec-17] ERROR [requestId=f9de91c6-ab1f] org.flywaydb.core.Flyway - Could not commit transaction: lock wait timeout exceeded
2026-05-26 23:59:34.650 [http-nio-8080-exec-14] ERROR [requestId=dbe7cece-1213] ru.da.gov.bank.service.AcquiringService - External API call failed: /api/v1/acquiring/charge -> 503 Service Unavailable
2026-05-26 23:59:42.777 [http-nio-8080-exec-4] ERROR [requestId=f71300b1-5a1b] ru.da.gov.bank.service.AcquiringService - External API call failed: /api/v1/auth/login -> 503 Service Unavailable
2026-05-26 23:59:56.493 [http-nio-8080-exec-21] ERROR [requestId=31f4bdd3-4242] com.zaxxer.hikari.pool.HikariPool - SQLException: duplicate key value violates unique constraint

# 4 Сколько Timeout в логе?
## Timeout: 2429
# 5 Топ 3 типа ошибок
## Самые популярные: 500 503 504
