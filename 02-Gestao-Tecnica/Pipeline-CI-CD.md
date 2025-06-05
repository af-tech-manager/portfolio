# ⚙️ Pipeline CI/CD: Etapas, Ferramentas e Boas Práticas
Por: [ Alan Fernandes - Tech Manager ] :house: [Voltar para home](https://github.com/af-tech-manager/portfolio/blob/main/README.md)

## Introdução
A entrega de software moderna exige velocidade, qualidade e automação. Nesse contexto, o uso de Pipelines CI/CD **(Continuous Integration / Continuous Delivery)** se tornou padrão nas equipes de alta performance.

Pipelines bem definidos garantem que o código entregue seja testado, validado, integrado e disponibilizado automaticamente, reduzindo falhas e acelerando o time-to-market.

## O que é CI/CD?
- **CI (Continuous Integration):** Processo de integrar alterações de código de todos os desenvolvedores de forma contínua, com automação de testes e validações.

- **CD (Continuous Delivery/Deployment):** Automatização da entrega ou implantação do software em ambientes controlados (homologação e produção).

## Etapas Comuns de um Pipeline CI/CD
| Etapa                              | Objetivo                                                  |
| ---------------------------------- | --------------------------------------------------------- |
| 1. **Build**                       | Compilar o código, resolver dependências                  |
| 2. **Testes**                      | Executar testes unitários, de integração, segurança, etc. |
| 3. **Análise Estática**            | Verificar qualidade do código, padrões e vulnerabilidades |
| 4. **Empacotamento**               | Gerar artefatos (ex: .jar, .zip, container)               |
| 5. **Deploy em HML**               | Publicar em ambiente de homologação para validação        |
| 6. **Testes Automatizados em HML** | Executar testes end-to-end (E2E), smoke tests             |
| 7. **Deploy em Produção**          | Entrega automática ou manual com rollback configurado     |
| 8. **Notificações e Logs**         | Comunicação com Slack, e-mail, dashboards                 |


## Ferramentas Comuns por Etapa
| Etapa        | Ferramentas sugeridas                                   |
| ------------ | ------------------------------------------------------- |
| Build/Test   | Maven, Gradle, npm, pip, JUnit, Jest, Mocha             |
| CI Servers   | GitHub Actions, GitLab CI, Jenkins, CircleCI, Travis CI |
| Análise      | SonarQube, ESLint, Pylint, CodeClimate                  |
| Containers   | Docker, Podman                                          |
| Orquestração | Kubernetes, Helm, ArgoCD                                |
| Deploy       | Ansible, Terraform, AWS CodeDeploy, Octopus Deploy      |
| Testes E2E   | Cypress, Selenium, Playwright                           |
| Notificações | Slack, MS Teams, Email, Grafana/Prometheus              |

## Exemplo Visual: Pipeline CI/CD
![image](https://github.com/user-attachments/assets/d574787b-d3d2-4850-9a18-1da6f935f971)

## Boas Práticas
✅ Mantenha o pipeline curto e confiável.

✅ Teste falhas de build e simule cenários de rollback.

✅ Utilize “feature flags” para liberar funcionalidades sem novos deploys.

✅ Implemente canary releases ou blue/green deployments.

✅ Automatize rollback e monitoramento após deploy.

✅ Documente seu pipeline e torne-o versionável.

## CI vs CD vs CD 🤔
Termo e significado:

- **CI (Integração Contínua):** Testar e validar código automaticamente.
- **CD (Entrega Contínua):** Entregar código aprovado em ambiente hml/prod.
- **CD (Implantação Contínua):** Deploy automático direto em produção (sem gatilhos manuais).

## Conclusão
Pipelines CI/CD são a coluna vertebral da engenharia moderna de software. Com eles, times ganham agilidade, previsibilidade e segurança na entrega contínua de valor ao cliente. \
\
Quando bem configurado, o pipeline se torna um aliado estratégico para o negócio.

---
:lock: 2025 - Todos os direitos autorais reservados à Alan Fernandes - pm.alfernandes@gmail.com
