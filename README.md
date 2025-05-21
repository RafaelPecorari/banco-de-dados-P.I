# Escolha do Banco de Dados Relacional

## Objetivo

Selecionar o banco de dados relacional mais adequado para a aplicação, considerando:

- Compatibilidade com as API's;
- Facilidade de instalação e manutenção;
- Simplicidade sem comprometer a robustez;
- Comunidade ativa e documentação acessível.

---

## Banco de Dados Escolhido: **MySQL**

### Por que escolhemos o MySQL?

**Vantagens:**

- Ampla compatibilidade com ORMs e frameworks backend como Sequelize (Node.js) e outros.
- Fácil de instalar, configurar e manter, o que o torna uma excelente escolha para equipes com diferentes níveis de experiência.
- Grande comunidade ativa e extensa base de conhecimento.
- Suporte a replicação, particionamento e outras funcionalidades para aplicações de médio a grande porte.
- Utilizado amplamente na indústria, inclusive em aplicações de grande escala como WordPress, Facebook e Shopify (MariaDB/MySQL).

**Decisão:**  
✅ **Escolhido como banco principal da aplicação.**  
É simples o suficiente para uso imediato e robusto o bastante para suportar a evolução do sistema.

---

## Outras Alternativas Avaliadas

### 1. **PostgreSQL**

**Vantagens:**

- Excelente suporte a tipos de dados avançados (como JSONB, arrays, enums).
- Muito robusto em termos de conformidade com o padrão SQL e integridade transacional.

**Desvantagens:**

- Requer curva de aprendizado um pouco maior.
- Administração e configuração mais complexa, especialmente em ambientes menos técnicos.

**Decisão:**  
❌ **Não escolhido.**  
Apesar de ser tecnicamente superior em alguns aspectos, optamos por uma solução mais simples e direta para o perfil da aplicação.

---

### 2. **SQLite**

**Vantagens:**

- Extremamente leve e fácil de usar.
- Ideal para prototipagem e testes locais.

**Desvantagens:**

- Não recomendado para ambientes multiusuário e aplicações web em produção.
- Falta de suporte a muitos recursos necessários em produção.

**Decisão:**  
❌ **Descartado para produção.**  
Pode ser útil para protótipos, mas não atende às necessidades da aplicação em produção.

---

## Conclusão

| Banco      | Compatibilidade | Simplicidade | Escalabilidade | Suporte a Recursos Avançados | Escolhido |
|------------|------------------|---------------|------------------|-------------------------------|-----------|
| MySQL      | ✅ Alta           | ✅ Alta        | ✅ Alta           | ⚠️ Média                      | ✅ Sim     |
| PostgreSQL | ✅ Alta           | ⚠️ Média       | ✅ Alta           | ✅ Excelente                   | ❌ Não     |
| SQLite     | ⚠️ Baixa          | ✅ Muito alta  | ❌ Baixa          | ⚠️ Limitado                   | ❌ Não     |

Portanto, **MySQL** foi escolhido por sua **facilidade de uso, ampla adoção no mercado e compatibilidade com a stack da aplicação**, sem comprometer os requisitos essenciais do sistema.
