# Azure-Cognitive-Search
Armazena projeto: Utilizando AI Search para indexação e consulta de Dados
Segue abaixo o passo a passo para se configurar uma pesquisa (vide https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html), assim como seus insights, possibilidades de ferramentas que se beneficiam com esse tipo de ferramenta e aprendizados adquiridos durante o processo.

Você é solicitado a ajudar a criar uma solução de mineração de conhecimento que facilite a pesquisa de insights sobre as experiências do cliente. Você decide criar um índice de Pesquisa de IA do Azure usando dados extraídos de avaliações de clientes.

1. Recursos do Azure necessários
A solução que você criará requer os seguintes recursos em sua assinatura do Azure:

> Um recurso de Pesquisa de IA do Azure, que gerenciará a indexação e a consulta.
> Um recurso de serviços de IA do Azure, que fornece serviços de IA para habilidades que sua solução de pesquisa pode usar para enriquecer os dados na fonte de dados com insights gerados por IA.

Nota Seus recursos de Pesquisa de IA do Azure e serviços de IA do Azure devem estar no mesmo local!

> Uma conta de armazenamento com contêineres de blob, que armazenará documentos brutos e outras coleções de tabelas, objetos ou arquivos.

Criar um recurso de Pesquisa de IA do Azure
Entre no portal do Azure.

Clique no botão + Criar um recurso, procure Pesquisa de IA do Azure e crie um recurso de Pesquisa de IA do Azure com as seguintes configurações:

Assinatura: sua assinatura do Azure.
Grupo de recursos: selecione ou crie um grupo de recursos com um nome exclusivo.
Nome do serviço: um nome exclusivo.
Localização: Escolha qualquer região disponível.
Nível de preços: Básico
Selecione Revisar + criar e, depois de ver a resposta Êxito da validação, selecione Criar.

Após a conclusão da implantação, selecione Ir para o recurso. Na página de visão geral da Pesquisa de IA do Azure, você pode adicionar índices, importar dados e pesquisar índices criados.

Criar um recurso de serviços de IA do Azure
Você precisará provisionar um recurso de serviços de IA do Azure que esteja no mesmo local que seu recurso de Pesquisa de IA do Azure. Sua solução de pesquisa usará esse recurso para enriquecer os dados no armazenamento de dados com insights gerados por IA.

Retorne à home page do portal do Azure. Clique no botão +Criar um recurso e procure serviços de IA do Azure. Selecione criar um plano de serviços de IA do Azure. Você será levado a uma página para criar um recurso de serviços de IA do Azure. Configure-o com as seguintes configurações:
Assinatura: sua assinatura do Azure.
Grupo de recursos: o mesmo grupo de recursos que seu recurso de Pesquisa de IA do Azure.
Região: o mesmo local que seu recurso de Pesquisa de IA do Azure.
Nome: Um nome exclusivo.
Nível de preços: Standard S0
Ao marcar esta caixa reconheço que li e compreendi todos os termos abaixo: Selecionado
Selecione Revisar + criar. Depois de ver a resposta Validação aprovada, selecione Criar.

Aguarde a conclusão da implantação e exiba os detalhes da implantação.
Criar uma conta de armazenamento
Retorne à home page do portal do Azure e selecione o botão + Criar um recurso.

Procure uma conta de armazenamento e crie um recurso de conta de armazenamento com as seguintes configurações:
Assinatura: sua assinatura do Azure.
Grupo de recursos: o mesmo grupo de recursos que os recursos da Pesquisa de IA do Azure e dos serviços de IA do Azure.
Nome da conta de armazenamento: um nome exclusivo.
Localização: Escolha qualquer local disponível.
Desempenho: Standard
Redundância: Armazenamento localmente redundante (LRS)
Clique em Rever e, em seguida, clique em Criar. Aguarde a conclusão da implantação e vá para o recurso implantado.

Na conta de Armazenamento do Azure que você criou, no painel de menu esquerdo, selecione Configuração (em Configurações).
Altere a configuração de Permitir acesso anônimo de Blob para Habilitado e selecione Salvar.


