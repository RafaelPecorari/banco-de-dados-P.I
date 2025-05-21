# Escolha do Banco de Dados Relacional

## Objetivo

Selecionar o banco de dados relacional mais adequado para a aplicação, considerando:

- Compatibilidade com a API Backend;
- Facilidade de instalação e manutenção;
- Simplicidade sem comprometer a robustez;
- Comunidade ativa e documentação acessível.

---

## 2. Por que escolhemos o MySQL?

**Compatibilidade com .NET:**  
MySQL possui suporte oficial através do **MySQL Connector/NET**, facilitando a integração com o C# e o **Entity Framework Core**, tornando o desenvolvimento mais eficiente e produtivo.

**Simplicidade e Eficiência:**  
É fácil de configurar e utilizar, ideal para projetos com necessidades moderadas como **cadastro de alunos, professores e gestão de demandas**.  

**Desempenho em Operações CRUD:**  
Excelente performance para operações de **Create, Read, Update e Delete**, principalmente com **dados textuais e caminhos de imagens**, comuns em sistemas acadêmicos.

---

## 3. Exemplos de Uso

**Cadastro de Alunos:**

- Utilização de transações para garantir a segurança dos dados.
- Consultas simples e eficientes para listagem por turma.
- Estrutura com tabelas como `alunos`, `cursos` e `matrículas`, com relacionamentos bem definidos.

**Gestão de Demandas:**

- Demandas associadas a professores e alunos.
- Consultas frequentes com **índices otimizados** para garantir boa performance.
- Uso consistente de **chaves estrangeiras** para manter a integridade dos dados.

---

## 4. Diferenciais do MySQL

- **Fácil manutenção** e **baixo consumo de recursos**.
- Boa performance mesmo em **máquinas simples**.
- Ampla **compatibilidade com aplicações web e desktop**, incluindo integração com .NET, Java e PHP.
- Comunidade ativa e excelente documentação.

---

## 5. Outras Alternativas Avaliadas

### PostgreSQL

**Prós:**

- Recursos avançados (JSONB, Arrays, Window Functions).
- Excelente conformidade com o padrão SQL.

**Contras:**

- Curva de aprendizado maior.
- Administração mais complexa.

**Motivo de não escolha:**  
Apesar de seus recursos avançados, o foco do projeto é em simplicidade e integração com .NET, onde o MySQL oferece melhor compatibilidade e facilidade de uso.

---

### SQLite

**Prós:**

- Leveza e facilidade de uso.
- Ideal para testes locais.

**Contras:**

- Não recomendado para ambientes com múltiplos usuários.
- Escalabilidade limitada.

**Motivo de não escolha:**  
Não atende aos requisitos de produção e concorrência de acessos do projeto.

---

## 6. Conclusão

O **MySQL** se mostrou uma excelente escolha para o nosso projeto por sua combinação de **eficiência, simplicidade e integração com o .NET**.

A estrutura do banco foi planejada para:

- Garantir a integridade dos dados com uso de chaves estrangeiras;
- Proporcionar boa performance com índices apropriados;
- Ser facilmente mantida, mesmo em ambientes de hardware limitado.

---

## Tabela Comparativa

| Banco      | Compatibilidade | Simplicidade | Escalabilidade | Recursos Avançados | Integração com .NET | Escolhido |
|------------|------------------|---------------|------------------|----------------------|-----------------------|-----------|
| MySQL      | ✅ Alta           | ✅ Alta        | ✅ Alta           | ⚠️ Média             | ✅ Excelente           | ✅ Sim     |
| PostgreSQL | ✅ Alta           | ⚠️ Média       | ✅ Alta           | ✅ Excelente         | ⚠️ Boa                 | ❌ Não     |
| SQLite     | ⚠️ Baixa          | ✅ Muito alta  | ❌ Baixa          | ⚠️ Limitado          | ⚠️ Limitada            | ❌ Não     |

---
criado por: Rafael pecorari de Barros
---
apresentado por : João Victor de Souza Santos
                  Rayan Luca Teixeira de Souza
