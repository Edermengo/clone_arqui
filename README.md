# clone_arqui
DOCUMENTO TÉCNICO - PROJETO CLONE ARQUIMEDES
1. FINALIDADE DO SISTEMA
O Arquimedes é um sistema destinado à elaboração, gerenciamento e impressão de orçamentos
de obras.
Funções principais:
- Criação de orçamentos organizados em capítulos, subcapítulos e serviços
- Inserção de serviços de bancos de preços públicos ou bases próprias
- Cálculo automático de custos e aplicação de BDI
- Geração de relatórios técnicos para licitações
2. ARQUITETURA DO SISTEMA
Tipo de Aplicativo: Desktop (Windows) ou Web
Linguagens sugeridas: C# (.NET) ou NodeJS + ReactJS
Banco de Dados: SQLite (local) ou MySQL (web)
3. ESTRUTURA DE FUNCIONAMENTO
Banco de Dados:
- obras(id, nome, local, data, licitação)
- capitulos(id, obra_id, titulo, ordem)
- servicos(id, capitulo_id, codigo, descricao, unidade, quantidade, preco_unitario, preco_total)
- bases_precos(id, banco, codigo, descricao, unidade, preco)
Fluxo de Uso:
- Tela Inicial: Criar/Abrir orçamento
- Editor de Orçamento: Planilha com capítulos/subcapítulos/serviços
- Banco de Preços: Consulta e importação
- Relatórios: Exportação para Excel e PDF
4. FUNCIONALIDADES PRINCIPAIS
- Criação de orçamentos
Page 1
Clone Arquimedes - Documento Técnico
- Organização hierárquica
- Banco de preços integrado
- Aplicação de BDI
- Geração de relatórios
5. INTERFACE DE USUÁRIO (UI)
- Menu lateral: Orçamentos | Banco de Preços | Relatórios | Configurações
- Área central: Tabela tipo grid
- Botões flutuantes: Adicionar Capítulo, Inserir Serviço, Exportar
6. TECNOLOGIAS SUGERIDAS
- Backend: C# .NET ou NodeJS
- Frontend: Windows Forms ou ReactJS
- Banco: SQLite ou MySQL
- Exportação: EPPlus, SheetJS, iTextSharp
RESUMO FINAL
O sistema Arquimedes é voltado para criar orçamentos de obras públicos e privados, organizados
em estrutura hierárquica, integrando banco de preços e gerando relatórios oficiais
