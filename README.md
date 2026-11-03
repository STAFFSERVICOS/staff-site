# STAFF — Site Institucional

Site institucional da **STAFF — Prestação de Serviços Administrativos LTDA**, desenvolvido como uma página estática, responsiva e de apresentação corporativa.

**Responsável pela implementação técnica:** João Paulo.

**Domínio institucional previsto:** https://staffservicos.com

> **Nota:** a configuração e a disponibilidade do domínio próprio devem ser verificadas separadamente. O endereço do GitHub Pages é a referência inicial do projeto.

## 1. Objetivo

Apresentar a empresa, seus serviços administrativos, dados institucionais e informações iniciais sobre privacidade. O site também foi planejado para apoiar a presença digital da empresa durante a configuração e a verificação empresarial junto à Meta, visando uma futura integração com a **WhatsApp Business Platform (Cloud API)** e um sistema de chamados.

**Importante:** este repositório contém somente o site institucional. **Não** implementa a API do WhatsApp, webhooks, banco de dados, autenticação nem o sistema de chamados. A verificação empresarial na Meta não é garantida pela publicação deste site.

## 2. Tecnologias e hospedagem

- **HTML5:** conteúdo e estrutura semântica.
- **CSS3:** identidade visual, layout responsivo e componentes de apresentação.
- **JavaScript:** atualização automática do ano no rodapé.
- **GitHub Pages:** hospedagem de arquivos estáticos, sem VPS ou backend.
- **DNS do domínio:** administrado separadamente; os serviços de e-mail Microsoft 365 devem ser preservados.

Não há dependências, compilação ou instalação de pacotes para a versão atual.

## 3. Estrutura dos arquivos

```text
staff-site/
├── index.html          # Página principal, estilos CSS e script do rodapé
├── staff-logo-1.png    # Logotipo usado no cabeçalho
├── staff-logo-2.png    # Logotipo usado no rodapé
├── favicon.png         # Ícone da aba do navegador
└── README.md           # Documentação do projeto
```

**Atenção:** os nomes e caminhos dos arquivos de imagem devem corresponder exatamente aos atributos `src` e `href` do `index.html`, inclusive em relação a maiúsculas e minúsculas. Os arquivos de imagem ficam na **raiz do repositório**, junto ao HTML.

## 4. Estrutura da página

O `index.html` está organizado em seções identificadas por âncoras:

| Âncora | Conteúdo |
| --- | --- |
| `#inicio` | Apresentação e chamada principal |
| `#sobre` | Informações sobre a STAFF |
| `#servicos` | Áreas de atuação administrativa |
| `#institucional` | Razão social, CNPJ e endereço |
| `#privacidade` | Informações preliminares sobre privacidade |
| `#contato` | Rodapé com informações institucionais e localização |

O menu utiliza links internos. O botão de contato, na versão atual, **não** envia mensagens nem abre um formulário: ele leva ao rodapé.

## 5. Identidade visual

A proposta visual é **clean, corporativa e responsiva**, com fundo predominantemente branco, textos em azul-marinho, detalhes em laranja associados à marca STAFF e tipografia sem serifa. Os logotipos fornecidos para o projeto são usados no cabeçalho e no rodapé.

As cores e regras de apresentação ficam no bloco `<style>` dentro de `index.html`, incluindo variáveis CSS no seletor `:root`. Alterações de identidade visual devem preferencialmente começar por essas variáveis.

## 6. Publicação e manutenção

1. Manter `index.html`, os PNGs e este `README.md` na raiz do repositório.
2. Acessar **Settings → Pages** no GitHub.
3. Selecionar **Deploy from a branch**, branch `main`, pasta `/ (root)`.
4. Salvar e aguardar a publicação.
5. Testar o endereço do GitHub Pages, o menu, a versão móvel e o carregamento dos logotipos.
6. Se houver domínio personalizado, configurar **Custom domain**, os registros DNS recomendados pelo GitHub e **Enforce HTTPS** quando disponível.

**Não modificar os registros MX, SPF, DKIM, DMARC ou Autodiscover do Microsoft 365** para publicar o site. Qualquer alteração de DNS deve ser precedida por conferência dos registros existentes.

## 7. Cuidados antes do uso definitivo

- Confirmar com a empresa que a descrição dos serviços, o endereço e os dados cadastrais estão atualizados.
- Substituir o texto **preliminar** da seção de privacidade por uma política completa e revisada, especialmente antes de coletar dados pessoais ou iniciar atendimento automatizado.
- Definir e divulgar canais oficiais de contato; não inserir números de telefone ou e-mails sem confirmação.
- Não armazenar senhas, tokens da Meta, segredos, dados de clientes ou outras credenciais neste repositório público.
- Se o atendimento WhatsApp for implementado, hospedar a API e os webhooks em um serviço backend apropriado, com HTTPS, validação de assinaturas, controles de acesso e tratamento seguro de dados.

## 8. Orientações para pessoas e assistentes de IA

Antes de modificar o projeto:

1. **Leia este README e o `index.html` completo.** Não presuma a existência de frameworks, arquivos ou serviços que não estejam no repositório.
2. **Preserve a identidade visual e os logotipos da STAFF.** Evite substituir a marca por imagens genéricas.
3. **Mantenha o site compatível com GitHub Pages.** Não introduza dependência obrigatória de backend sem justificar e documentar a mudança.
4. **Não invente dados empresariais.** Confirme contatos, serviços e informações legais antes de publicá-los.
5. **Não confunda o site com o projeto de API WhatsApp.** A integração de chamados é um objetivo futuro, não uma funcionalidade existente neste código.
6. **Evite mudanças destrutivas.** Prefira alterações incrementais, explique os arquivos afetados e teste responsividade, navegação e imagens.
7. **Respeite a privacidade.** Não inclua dados pessoais de clientes, credenciais ou informações confidenciais no HTML ou no histórico Git.
8. **Documente mudanças relevantes** neste arquivo para facilitar a continuidade do projeto.

## 9. Histórico e próximos passos

**Estado documentado:** versão institucional estática com layout clean, seções informativas e logotipos em arquivos PNG na raiz do repositório.

**Próximas atividades planejadas:**

- Concluir a associação do domínio `staffservicos.com` ao GitHub Pages e validar HTTPS.
- Revisar conteúdo institucional e publicar política de privacidade definitiva.
- Continuar a verificação empresarial na Meta.
- Projetar separadamente a integração oficial da Cloud API do WhatsApp ao sistema de chamados, avaliando a preservação do número existente por meio de Coexistence, quando elegível.

---

**Documentação do projeto:** João Paulo — implementação técnica e organização do site institucional da STAFF.
