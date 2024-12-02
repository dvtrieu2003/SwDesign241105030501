# Subsystem context diagrams
Một số hệ thống con: BankSystem, PrintService, ProjectManagementDatabase subsystems
- Hệ thống con BankSystem
![](https://www.planttext.com/api/plantuml/png/j5HBRiCW4Dtx5ADicaZD1ImhYjAaKZPLrIohBZ2Un2WOBC1ghAedww97wXKA-5Di9ykoi81vRzxC0_ppzRtMXYXJ5Jmop7243H5dEDJQO04FKXYyc2Wg2JsJ4yBiIdG67n7OSGTxkrP7GX6EKe791yayXlM8lGkrYHf-CumYGXzHFLOYqtD2gQo4UQgA55KC1wEOEDq3ATnk35jPfHpl6nAXXacn9GPjm7uNCMoav4Y4J_yPjLMwifNa71LGJhJsstu6pwHsaG2H9BHVh5Q3IaibAMfjEGKACryCLNR2sbctUPqTkwBaiaQ4bX38Tg4sOaNHitl1FcjelwvItSni9PTwqanWS9ACmADM_j_qrjckzXl6_vNh9zF-Nv0J9wXpLZRywP4jNtEMPIZUbglmbjr23r4GGwNnPceB7X-M9PIPxRpXZAEECMmk1gQxkuCPf7MerMAkwtIaHYceUTg3VsVsR3IyCvDx_7v429onzgvHPEuVy0i00F__0m00)
- Hệ thống con PrintService
![](https://www.planttext.com/api/plantuml/png/h5FBJiCm4BpdArQzq4hq1wAege0UUglQ8-BWEbjYrR53l856Y2_Zm2Vn2zYE4-NHtl39oUpCpexjt--VjI5MKfNBY0H9X5qf5C41otV14Hwr8hnG51MCdzahmkmgFeFF2EowWwtzBa_CGYTT0cKZGLybkfgj1rknHgDPXGDshEOPylCSyqBg6Z66JTZT0yjrfIY69rqT9IvYUD1Q8bDUv2iAVfp1Kak99N39ZF6__GwikaDw5Kd2ku_LQkH7SpJ6-ztZMuM6vejXguso2TP1t4tVUdMTSbJKwzr20R6TqRExhftgC6zJ7Krj27Ddw59FP-hdcIIZyibC_vDn218EJQiREGVKclARwQHxb8o4LYOJHSEVdj3oEHDfYkfbkHfUdblrupg8eJ9uKzwMZu_64egKKU2CKSSO3XY3CErrmHIETRzNgBdUfoK5TttNr-RmpuXnCl0XAFESxOGqoCX6lKQLkiV-1m00__y30000)
- Hệ thống ProjectManagementDatabase subsystems
![](https://www.planttext.com/api/plantuml/png/l5JDJeD04Bxp59DUR0zz0K98azP34pMDzMOyBCiKLc4XkqCiCJwP1n_9Lt1PVYoqe2SvxRBVptmp2ryVdojDJ56H9Wu9IX1sAdj6Jd3B98imHKcmOSG2fX7McIGyakFaZB-OKvZz0Js3DmVCSmLRirS7nX4EcGAA9yqiHtICRGFzGNO-jNpzH4ZhcAa8xueqGANd2nTkX2PlJqh8oEz36yqD4XE9dlCJfWirm_0RbAM-EqsMAfpAaWGLy8HfRL_R5Jo853bJuGd4ytYtyVrUnRdAE6hTakQBli-rD6Cf6-MgRItmWg6nGGllB3gPgJdf8j2b9aohMexbMPxnpdlUW3l8zc_JsB6oQYxiwrhE4jJ7pQcfsYxEktIF2IEHIHsBlEPVcENoCHPXYF9fwK_Sob7s90jSA3IEMnjoDsm3pKD60xJ5zFEw87HxpJ24eBI4FcQWtA9hxV5oVqrZFs36ISEheDYgJU1jxQCTDMDQeGohNzKt0000__y30000)
# Mapping Analysis Class to Design Element


| **Analysis Class**               | **Design Element**                     |
|----------------------------------|----------------------------------------|
| **PayrollController**            | PayrollController (control)            |
| **IBankSystem**                  | IBankSystem (interface)                |
| **BankSystem**                   | BankSystem (subsystem proxy)           |
| **EmployeePayment**              | EmployeePayment (entity)               |
| **IPrintService**                | IPrintService (interface)              |
| **PrintService**                 | PrintService (subsystem proxy)         |
| **IProjectManagementDatabase**   | IProjectManagementDatabase (interface) |
| **ProjectManagementDatabase**    | ProjectManagementDatabase (subsystem proxy) |
| **ProjectInfo**                  | ProjectInfo (entity)                   |
# Mapping Design Element to Owning Package

| Design Element                | Owning Package                  |
|-------------------------------|----------------------------------|
| **PayrollController**          | payroll.controller               |
| **IBankSystem**                | payroll.bank.interface           |
| **BankSystem**                 | payroll.bank.subsystem           |
| **EmployeePayment**            | payroll.entity                   |
| **IPrintService**              | payroll.print.interface          |
| **PrintService**               | payroll.print.subsystem          |
| **IProjectManagementDatabase** | payroll.project.interface        |
| **ProjectManagementDatabase**  | payroll.project.subsystem        |
| **ProjectInfo**                | payroll.entity                   |

# Architectural Layers and Dependencies
![](https://www.planttext.com/api/plantuml/png/X5J1JW8n4BttAoPUFF43X10GF91W92Wduw6KWMtejhNJ1OdnoppuIVw2xOAukDtrjctVcpTlNhjV7vy3yjpv8bUCjbA3CuJi6iQubXh1PmYA7z0HSBq2ON9hD6fFZ5akjdo3S3LpI66BUsaqJ2Fu2juOmDDYyWoztfdJxyVDaT7U6QNG9Gw7imcCb0phluVl5S6XjKgAkjvDGQ5d8fYQZHJmW6ud1QPaAWKQK5MzCVVyGcYErf3qnXqInIDwoIcbUp-_QzEPQ8yRL_Tr--hHQQwWUJm1zPX9ju9PoFBGOkgSh4DLAb4cBS4I_HvHdx9cPNITJhzvfbsGeLl7XIVOIv-nYs1BQdBAaRSpMmmQLJTj1C6L2l2cJafgDP4kl1Je91AiGXGiNJR1ikZMnkK4e_bY32OiZmDY5xYI-9jnVGurS9bw5meA7OLl229HYoHvr0B_SPOC_pGKm9z3EdBQp3OLCdbUw4Z1euFmvkD5il4YCJP0lOh_Xcy0003__mC0)
