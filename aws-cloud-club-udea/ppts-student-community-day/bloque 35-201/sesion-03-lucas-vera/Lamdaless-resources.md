# Lambdaless: Serverless sin Lambda
**AWS Student Community Day Colombia 2025**

## Resumen
Esta es una charla de arquitecturas serverless. El objetivo es revisar cuándo **NO** necesitas una Lambda: validaciones en API Gateway, orquestación declarativa con Step Functions y resolvers/pipelines en AppSync. Verás patrones prácticos para **quitar Lambdas** que solo “pasan datos”, reduciendo *cold starts*, costo y artefactos a mantener.

## Agenda
- Serverless y Lambda (contexto)
- Caso 1: API Gateway con integración directa (CRUD)
- Caso 2: Step Functions para post-pago (orquestación sin “lambda-lith”)
- Caso 3: AppSync con pipeline resolvers e invocación de Step Functions
- Conclusiones y preguntas  

## Público objetivo
Estudiantes, desarrolladores y arquitectos con nociones básicas de AWS que deseen construir APIs y flujos **serverless** con menos código y de manera declarativa.

---

## Recursos por sección

### General
- [Aniversario de 10 años de Lambda](https://aws.amazon.com/serverless/10th-anniversary/)
- [Serverless Land 10 años de lambda](https://www.youtube.com/watch?v=AJaJk9I94Kk)
- [Mejores practicas para desarrolladores serverless](https://www.youtube.com/watch?v=5wokwEtddtc)
- [Construyendo aplicaciones serverless con AWS SAM](https://www.youtube.com/watch?v=jZcS-XRt2Mo)
- [Integraciones directas en aplicaciones serverless](https://docs.aws.amazon.com/wellarchitected/latest/serverless-applications-lens/direct-integrations.html)
- [Serverless Land](https://serverlessland.com/)

### API Gateway
- [Qué es API Gateway](https://docs.aws.amazon.com/apigateway/latest/developerguide/welcome.html)
- [Integraciones en API Gateway](https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-develop-integrations-aws-services.html)
- [Integración de API Gateway a DynamoDb](https://serverlessland.com/patterns/apigw-dynamodb)
- [Serverless API Sin Lambda](https://www.andmore.dev/blog/build-serverless-api-with-no-lambda/)

### Step Functions
- [Qué es Step Functions](https://docs.aws.amazon.com/step-functions/latest/dg/welcome.html)
- [Integraciones de Step Functions](https://docs.aws.amazon.com/step-functions/latest/dg/integrate-services.html)
- [Patrones avanzados de Step Functions](https://www.youtube.com/watch?v=gdGgBKJiM2E)

### AppSync
- [Qué es AppSync](https://docs.aws.amazon.com/appsync/latest/devguide/what-is-appsync.html)
- [AppSync Resolvers en Javascript](https://docs.aws.amazon.com/appsync/latest/devguide/resolver-reference-overview-js.html)
- [AppSync Resolvers HTTP](https://docs.aws.amazon.com/appsync/latest/devguide/resolver-reference-http-js.html)
- [AppSync Resolvers DynamoDB](https://docs.aws.amazon.com/appsync/latest/devguide/tutorial-dynamodb-resolvers.html)
- [Invocar Step Functions desde AppSync](https://aws.amazon.com/blogs/mobile/invoking-aws-step-functions-short-and-long-running-workflows-from-aws-appsync/)

---


## ¿Cuándo sí usar Lambda?
- Lógica de negocio compleja, SDKs propietarios, validaciones no triviales, o cuando el equipo sea más productivo en código que en configuración declarativa. *(Discutido en la charla; ver slides).*

## Contacto
**Lucas Vera Toro**
- [Blog](https://blog.lucasdev.info/)
- [LinkedIn](https://www.linkedin.com/in/lucas-vera-toro-1355b479/)
- [Repo con código de la charla](https://github.com/LucasVera/Lambdaless-APIs)

## Licencia
Este material, incluyendo el código fuente, slides y demos, se comparten con **fines educativos y no comerciales**
