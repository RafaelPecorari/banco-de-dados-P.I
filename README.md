
Escolha do Banco de Dados Relacional

Objetivo

Selecionar o banco de dados relacional mais adequado para a aplicação, levando em conta:

- Compatibilidade com a API 
- Facilidade de uso e simplicidade na administração;
- Capacidade de atender às necessidades do sistema com confiabilidade e desempenho;
- Comunidade ativa e boa documentação.

---

## opções analisadas: 

### 1. **PostgreSQL**

**Vantagens:**

- Totalmente compatível com ORMs populares como Sequelize (Node.js), SQLAlchemy (Python), Hibernate (Java), entre outros.
- Suporte a tipos avançados de dados como JSON, arrays e enums.
- Excelente suporte para integridade relacional, constraints e transações.
- Comunidade ativa e extensa documentação.
- Escalável e seguro, com recursos robustos como controle de concorrência multiversão (MVCC).

**Desvantagens:**

- Pode ser um pouco mais complexo de configurar em comparação com bancos mais simples, como SQLite.

**Decisão:**  
✅ **Escolhido como principal banco de dados.**  
É robusto, moderno e altamente compatível com diferentes stacks de desenvolvimento. Ideal para aplicações que podem crescer e se tornar mais complexas ao longo do tempo.

---

### 2. **MySQL**

**Vantagens:**

- Muito utilizado em projetos web tradicionais (LAMP stack).
- Boa compatibilidade com ferramentas populares e ORMs.
- Fácil de instalar e administrar.
- MariaDB, como fork, é 100% compatível com MySQL e tem desenvolvimento aberto.

**Desvantagens:**

- Recursos mais limitados que o PostgreSQL em alguns aspectos avançados.
- Suporte a conformidade com o padrão SQL não é tão rigoroso quanto o PostgreSQL.

**Decisão:**  
🟡 **Alternativa viável, mas não escolhida.**  
Embora seja simples e popular, o PostgreSQL oferece mais vantagens para aplicações modernas que exigem flexibilidade e recursos avançados.

---

### 3. **SQLite** 
**Vantagens:**

- Extremamente leve e simples.
- Ideal para protótipos, testes ou aplicações locais.

**Desvantagens:**

- Não recomendado para aplicações web com múltiplos usuários simultâneos.
- Pouco escalável.

**Decisão:**  
🔴 **Descartado para produção.**  
Pode ser útil para testes locais ou protótipos, mas não atende à necessidade de um sistema multiusuário em produção.

---

## Conclusão

| Banco      | Compatibilidade | Simplicidade | Escalabilidade | Suporte a Recursos Avançados | Escolhido |
|------------|------------------|---------------|------------------|-------------------------------|-----------|
| PostgreSQL | ✅ Alta           | ⚠️ Média       | ✅ Alta           | ✅ Excelente                   | ✅ Sim     |
| MySQL      | ✅ Alta           | ✅ Alta        | ✅ Alta           | ⚠️ Média                      | ❌ Não     |
| SQLite     | ⚠️ Baixa          | ✅ Muito alta  | ❌ Baixa          | ⚠️ Limitado                   | ❌ Não     |

Portanto, **PostgreSQL** foi a melhor escolha considerando **equilíbrio entre simplicidade, robustez e compatibilidade** com diferentes tecnologias de backend.
