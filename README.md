# case_techway

# Notas sobre Problemas e Soluções - task chave: OSD-2368

## Arquivos Estáticos
- **Descrição do Problema:** Os arquivos estáticos não estavam sendo servidos corretamente, impactando o carregamento de estilos e imagens.
- **Solução Aplicada:** Configuração ajustada em `jj_investimento/settings.py` para direcionar o Django ao usar recursos estáticos. Adicionado caminho `STATICFILES_DIRS` para incluir a pasta `page_app/static` como um diretório de arquivos estáticos.

## Nomes Incorretos de Imagens
- **Descrição do Problema:** Alguns nomes de imagens estavam incorretos.
- **Solução Aplicada:** Renomeadas as imagens corretamente no diretório `page_app/static/page_app/img/`.

## Links do Rodapé
- **Descrição do Problema:** Os links do rodapé estavam apontando para marcadores não definidos.
- **Solução Aplicada:** Corrigidas as referências dos links do rodapé em `page_app/templates/page_app/partial/footer.html`.

## Caminho da Imagem do Logotipo
- **Descrição do Problema:** O caminho da imagem do logotipo no cabeçalho estava usando um caminho absoluto.
- **Solução Aplicada:** Ajustado o tratamento para arquivos estáticos no caminho da imagem do logotipo em `page_app/templates/page_app/partial/header.html`.

## Caminho das Imagens na Página Inicial
- **Descrição do Problema:** Os caminhos das imagens na página inicial não estavam considerando os arquivos estáticos.
- **Solução Aplicada:** Ajustados os caminhos e tratamento para arquivos estáticos nas imagens da página inicial em `page_app/templates/page_app/partial/home.html`.

## Rota para "Nossos Serviços"
- **Descrição do Problema:** Não havia uma rota definida para a página "Nossos Serviços".
- **Solução Aplicada:** Adicionado caminho para a renderização da página "Nossos Serviços" em `page_app/urls.py`.

## Atualização das Informações de Contato
- **Descrição do Problema:** As informações de contato na página "contato.html" estavam desatualizadas, contendo endereço de e-mail, número de telefone e link do WhatsApp incorretos.
- **Solução Aplicada:** Atualizadas as informações de contato, corrigindo o endereço de e-mail para "contato@jjinvestimento.com.br", ajustando o link do WhatsApp para o número +1 (25) 2680-4187 e atualizando o número de telefone para +55 (41) 3223-2112.
