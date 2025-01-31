# Modelo Dimensional - Star Schema para Cenários de Vendas com Professores

## Descrição do Projeto
Este repositório contém a modelagem dimensional do **Star Schema** focado na análise dos **dados dos professores**. O objetivo é organizar e estruturar os dados de forma eficiente para facilitar consultas analíticas e relatórios gerenciais.

O modelo foi implementado em **MySQL** e pode ser utilizado para visualização e análise no **Power BI** ou outras ferramentas de BI.

---

## 📌 Estrutura do Star Schema

O modelo é composto por:

### **📂 Tabela Fato (`f_Professor`)**
Armazena os principais eventos e métricas, conectando as tabelas dimensão.

- `idProfessor` (FK) - Identificador do professor
- `idCurso` (FK) - Identificador do curso ministrado
- `idDepartamento` (FK) - Identificador do departamento
- `CursoMinistrado` - Nome do curso
- `CargaHoraria` - Tempo total do curso ministrado
- `Dt_Inicio` - Data de início do curso
- `Dt_Termino` - Data de término do curso

### **📂 Tabelas Dimensão**

#### **📌 `d_Professor` - Informações dos Professores**
- `idProfessor` (PK) - Identificador do professor
- `Nome` - Nome do professor
- `Formacao` - Nível de formação acadêmica
- `DataNasc` - Data de nascimento
- `DataFormacao` - Data de formação

#### **📌 `d_Curso` - Detalhes dos Cursos**
- `idCurso` (PK) - Identificador do curso
- `Nome` - Nome do curso
- `Categoria` - Categoria do curso (ex: Matemática, Física, Computação)
- `CargaHoraria` - Duração do curso

#### **📌 `d_Departamento` - Departamentos Acadêmicos**
- `idDepartamento` (PK) - Identificador do departamento
- `Nome` - Nome do departamento
- `Campus` - Localização do campus
- `Coordenador` - Nome do coordenador responsável

#### **📌 `d_Calendario` - Dimensão de Tempo**
- `Data` (PK) - Data específica para análise temporal

---

## 📊 Modelo Conceitual

O modelo **Star Schema** está representado no arquivo **[Star_Professor.pdf](https://github.com/Rodrigo-Antonio-Silva/Star-Schema/blob/main/Star_Professor.pdf)** disponível neste repositório.

---

## 📂 Arquivos do Repositório
- **`Star_Professor.pdf`** - Modelo em PDF com o diagrama do Star Schema
- **`README.md`** - Documentação do projeto

📬 Caso tenha dúvidas ou sugestões, entre em contato!

---

✍ **Desenvolvido por Rodrigo** 🚀
