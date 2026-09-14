---
layout: default
title: Política de Privacidade - HortPay
---

# Política de Privacidade — HortPay

**Última atualização: 14 de setembro de 2026**

**Aplicativo: HortPay — Controle de Vendas, Cultivos, Estoque e Financeiro**  
**Desenvolvedor: Jorge Fernando do Nascimento Rodrigues**  
**Contato: gestaodeestufashf@gmail.com**

---

## 1. Introdução

**Esta Política de Privacidade descreve como o aplicativo HortPay ("aplicativo", "nós") trata as informações do usuário ("você") durante a utilização de nossos serviços.**

**Respeitamos sua privacidade e nos comprometemos com a proteção de seus dados pessoais em conformidade com:**

- **Lei Geral de Proteção de Dados (LGPD — Lei nº 13.709/2018);**
- **Políticas de Privacidade e Segurança do Google Play.**

**Ao instalar e utilizar o HortPay, você concorda com as práticas descritas nesta Política.**

---

# 2. Dados que Coletamos

## 2.1. Dados armazenados exclusivamente no seu dispositivo

**O HortPay foi desenvolvido com o conceito offline-first. Por padrão, todos os dados operacionais permanecem armazenados localmente no dispositivo, utilizando banco de dados SQLite.**

**Salvo quando você ativa voluntariamente o Backup na Nuvem (Seção 2.2), nenhuma dessas informações é enviada para servidores externos.**

**Os dados armazenados localmente incluem:**

- **Cadastros de cultivos e áreas de plantio, incluindo ciclos de produção;**
- **Registros de vendas (produtos, compradores, caixas, preços e datas);**
- **Controle de estoque de insumos, categorias, quantidades, valores e movimentações FIFO;**
- **Aplicações foliares e fertirrigação;**
- **Custos de cultivo;**
- **Análises de solo e recomendações agronômicas;**
- **Contas a Pagar e Contas a Receber;**
- **Parcelamentos financeiros;**
- **Categorias financeiras personalizadas;**
- **Datas de emissão, vencimento e pagamento;**
- **Fluxo de Caixa (entradas, saídas e saldo);**
- **Saldo Inicial (dinheiro e contas bancárias);**
- **Cartões de crédito cadastrados contendo apenas: apelido, bandeira, banco, últimos quatro dígitos (opcional), dia de fechamento, dia de vencimento e limite total;**
- **Notificações locais de vencimento;**
- **Configurações locais, incluindo PIN de segurança, biometria (opcional) e preferências do usuário.**

**Nunca armazenamos:**

- **Número completo do cartão;**
- **Código CVV;**
- **Senha do cartão;**
- **Nome do titular.**

---

## 2.2. Backup na Nuvem e Login com Conta Google (opcional)

**O HortPay oferece um recurso opcional de Backup na Nuvem via Google Drive.**

**Esse recurso só é ativado quando você decide entrar com sua conta Google dentro do aplicativo.**

### a) Login com Conta Google

**A autenticação é feita pelo protocolo OAuth 2.0 do Google, por meio do navegador do sistema.**

**Ao entrar, o aplicativo recebe e armazena localmente no dispositivo, no armazenamento seguro do sistema (SecureStore), apenas:**

- **Seu e-mail da conta Google;**
- **Seu nome, usado, por exemplo, para a saudação no início do aplicativo;**
- **Sua foto de perfil, quando disponível;**
- **Tokens de acesso e de atualização (access/refresh token), que permitem manter a sessão e enviar backups sem solicitar o login a cada vez.**

### b) Escopo de acesso ao Google Drive

**O aplicativo solicita exclusivamente o escopo drive.appdata, que dá acesso somente a uma pasta privada e exclusiva do HortPay (a AppData folder), invisível no seu Google Drive e inacessível a outros aplicativos.**

**O HortPay não acessa, lê ou modifica nenhum outro arquivo, foto ou documento do seu Google Drive.**

### c) O que é enviado ao Google Drive

**Quando você faz um backup, manual ou automático, o arquivo de backup em formato JSON, contendo os dados operacionais descritos na Seção 2.1, é enviado por conexão criptografada (HTTPS) para essa pasta privada do aplicativo na sua própria conta do Google Drive.**

**Esse arquivo fica sob seu controle e sua conta. O desenvolvedor não tem acesso a ele.**

### d) Backup automático

**Você pode ativar backups automáticos, diário ou semanal.**

**Quando ativados, o aplicativo envia silenciosamente o backup à sua pasta privada do Google Drive nos intervalos escolhidos, mantendo um número limitado das versões mais recentes.**

**Você pode, a qualquer momento, sair da conta ou revogar o acesso do HortPay à sua conta Google diretamente no aplicativo, o que apaga os tokens e dados da conta salvos no dispositivo, e/ou através do endereço:**

[**https://myaccount.google.com/permissions**](https://myaccount.google.com/permissions)

---

## 2.3. Dados processados pelo Google Play

**Quando você realiza a assinatura do Plano Mensal, o pagamento é processado integralmente pelo Google Play Billing.**

**Nesse processo, o Google processa as informações de pagamento e sua conta Google, além de controlar o histórico da assinatura.**

**O HortPay recebe apenas um token anônimo informando se a assinatura está ativa.**

**Não temos acesso a cartões de crédito, contas bancárias ou dados financeiros da compra.**

**Para mais informações, consulte a Política de Privacidade do Google.**

---

## 2.4. Dados que NÃO coletamos

**O HortPay não coleta:**

- **Localização (GPS);**
- **Lista de contatos;**
- **Histórico de chamadas;**
- **Histórico de mensagens;**
- **Fotos ou arquivos do dispositivo, exceto quando você seleciona um arquivo JSON para restauração;**
- **Dados de telemetria;**
- **Dados analíticos de uso;**
- **Identificadores de publicidade;**
- **Número completo de cartões de crédito, CVV ou senhas de cartões;**
- **Qualquer dado da sua conta Google além do e-mail, nome e foto descritos na Seção 2.2, e somente quando você faz login voluntariamente.**

---

# 3. Permissões do Aplicativo

**O HortPay utiliza apenas as permissões necessárias ao funcionamento do aplicativo:**

- **Google Play Billing — processar a assinatura mensal;**
- **Acesso à Internet — utilizado apenas para:**
  - **Login com a conta Google;**
  - **Envio e restauração de backups na sua pasta privada do Google Drive;**
  - **Validação da assinatura.**

**Nenhum dado é transmitido para servidores do desenvolvedor.**

- **Notificações — exibir lembretes locais de vencimento de Contas a Pagar e Contas a Receber. Todas as notificações são geradas localmente no dispositivo;**
- **Reinicialização do aparelho (RECEIVE_BOOT_COMPLETED) — recriar automaticamente as notificações locais após o dispositivo ser reiniciado;**
- **Vibração e ativação temporária da tela (VIBRATE / WAKE_LOCK) — utilizadas apenas durante a entrega das notificações locais;**
- **Biometria — opcional; utilizada somente quando ativada manualmente por você;**
- **Arquivos JSON — importar e restaurar backups. Os arquivos permanecem sob seu controle.**

---

# 4. Como Utilizamos os Dados

**Os dados são utilizados exclusivamente para:**

- **Exibir informações cadastradas;**
- **Permitir edição dos registros;**
- **Gerar relatórios;**
- **Gerar arquivos PDF;**
- **Gerar planilhas Excel;**
- **Exportar arquivos CSV;**
- **Exportar e importar arquivos JSON;**
- **Calcular saldo financeiro, parcelas, vencimentos e fluxo de caixa;**
- **Exibir notificações locais;**
- **Controlar assinatura e período de teste;**
- **Quando você ativar o Backup na Nuvem, autenticar sua conta Google e enviar/restaurar o backup na sua pasta privada do Google Drive.**

**Nunca utilizamos seus dados para:**

- **Publicidade;**
- **Compartilhamento com terceiros;**
- **Marketing;**
- **Análise comportamental;**
- **Treinamento de Inteligência Artificial;**
- **Venda ou monetização de dados.**

---

# 5. Compartilhamento de Dados

**Não compartilhamos seus dados pessoais.**

**Como o aplicativo funciona primariamente offline, o desenvolvedor não tem acesso aos registros armazenados no seu dispositivo nem aos backups salvos na sua conta Google.**

### Exceções

**Poderá ocorrer compartilhamento apenas quando:**

- **Você enviar informações voluntariamente ao suporte por e-mail; ou**
- **Houver determinação judicial.**

---

## 5.1. Serviços de Terceiros

| **Serviço** | **Finalidade** | **Dados acessados** |
|---|---|---|
| **Google Play Billing** | **Processamento da assinatura** | **Conta Google e pagamento** |
| **Google Play Services** | **Distribuição e atualização do aplicativo** | **Dados padrão do Android** |
| **Login com Google (Google Identity / OAuth 2.0)** | **Autenticar você para o Backup na Nuvem** | **E-mail, nome e foto de perfil** |
| **Google Drive API (escopo drive.appdata)** | **Guardar/restaurar backups em pasta privada do aplicativo** | **Somente o arquivo de backup do HortPay** |

**Esses serviços possuem suas próprias Políticas de Privacidade.**

---

# 6. Backup e Exportação de Dados

**O HortPay oferece:**

- **Backup local (JSON): salvo no dispositivo, sob sua inteira responsabilidade;**
- **Backup na Nuvem (opcional): enviado à sua pasta privada no Google Drive, conforme descrito na Seção 2.2.**

**Ambos contêm:**

- **Cultivos;**
- **Ciclos;**
- **Vendas;**
- **Estoque;**
- **Movimentações FIFO;**
- **Custos;**
- **Aplicações;**
- **Análises de solo;**
- **Lançamentos financeiros;**
- **Parcelas;**
- **Categorias financeiras;**
- **Cartões cadastrados (apenas metadados);**
- **Fluxo de Caixa;**
- **Saldo Inicial;**
- **Configurações.**

### Importante

**O arquivo de backup em JSON é legível. Qualquer pessoa que possuir o arquivo poderá visualizar seus dados financeiros e históricos.**

**O backup local fica apenas no dispositivo. O backup na nuvem fica na sua conta Google, à qual o desenvolvedor não tem acesso.**

**Compartilhe arquivos de backup somente com pessoas autorizadas.**

**Recomendação: realize backups com frequência.**

**A desinstalação do aplicativo remove os dados locais e não existe recuperação pelo desenvolvedor. Os backups na nuvem permanecem na sua conta Google até que você os apague.**

---

# 7. Retenção e Exclusão de Dados

**Os dados locais permanecem enquanto o aplicativo estiver instalado.**

**Ao desinstalar, o Android remove automaticamente os dados locais.**

**Também é possível apagar manualmente em:**

**Configurações → Aplicativos → HortPay → Armazenamento → Limpar Dados**

### Dados da conta Google e da nuvem

**Você pode, dentro do aplicativo, sair da conta ou revogar o acesso, o que apaga tokens e dados da conta do dispositivo.**

**Os arquivos de backup na sua pasta privada do Google Drive podem ser removidos pelo próprio aplicativo ou mediante a revogação do acesso do HortPay em:**

[**https://myaccount.google.com/permissions**](https://myaccount.google.com/permissions)

---

## 7.1. Cancelamento da Assinatura

**O cancelamento pode ser realizado diretamente pela Google Play.**

**Após o cancelamento:**

- **O acesso permanece ativo até o término do período contratado;**
- **Não existe taxa de cancelamento;**
- **Cancelamentos durante o período de teste gratuito não geram cobrança;**
- **Os dados permanecem disponíveis em modo somente leitura.**

---

# 8. Segurança

**Adotamos medidas para proteger seus dados:**

- **PIN opcional de quatro dígitos e biometria opcional;**
- **Armazenamento local protegido pelos mecanismos de segurança do Android;**
- **PIN e tokens da conta Google armazenados no SecureStore do sistema;**
- **Dados de cartões armazenados apenas como metadados;**
- **Comunicação com o Google, incluindo login e Drive, feita exclusivamente por HTTPS, utilizando o fluxo OAuth 2.0 com PKCE;**
- **Acesso ao Google Drive limitado ao escopo drive.appdata, correspondente à pasta privada do aplicativo, sem acesso a outros arquivos do seu Drive.**

### Recomendações de segurança

**Recomendamos:**

- **Manter o Android atualizado;**
- **Não compartilhar seu PIN;**
- **Ativar a biometria;**
- **Realizar backups frequentes;**
- **Não compartilhar arquivos JSON com pessoas não autorizadas.**

**Embora adotemos boas práticas, nenhum sistema é totalmente invulnerável.**

---

# 9. Público-Alvo e Crianças

**O HortPay é destinado a usuários maiores de 18 anos que desejam administrar atividades agrícolas.**

**Não coletamos intencionalmente dados de menores.**

**Caso um responsável identifique utilização indevida, poderá entrar em contato conosco.**

---

# 10. Seus Direitos (LGPD)

| **Direito** | **Como funciona no HortPay** |
|---|---|
| **Acesso** | **Os dados permanecem no seu dispositivo e, se ativado, na sua conta Google** |
| **Correção** | **Pode ser realizada diretamente no aplicativo** |
| **Exclusão** | **Desinstalar o aplicativo / limpar dados; revogar o acesso Google para dados da nuvem** |
| **Portabilidade** | **Disponível através do Backup JSON, local ou na nuvem** |
| **Revogação do consentimento** | **Sair da conta Google no aplicativo e/ou interromper o uso e desinstalar** |

---

# 11. Alterações nesta Política

**Esta Política poderá ser atualizada periodicamente.**

**Quando isso ocorrer:**

- **A data da última atualização será alterada;**
- **Alterações relevantes serão comunicadas dentro do aplicativo;**
- **A versão mais recente permanecerá disponível junto ao aplicativo.**

---

# 12. Contato e Encarregado de Dados

**E-mail de suporte:**  
gestaodeestufashf@gmail.com

**Aplicativo:**  
HortPay v1.0.91 — Android

**Prazo médio de resposta:**  
Até 15 (quinze) dias úteis.

**Autoridade Nacional de Proteção de Dados (ANPD):**  
https://www.gov.br/anpd

---

# Conformidade

**Esta Política foi elaborada em conformidade com:**

- **Lei Geral de Proteção de Dados (LGPD);**
- **Políticas de Dados e Privacidade da Google Play;**
- **Diretrizes de Transparência para Aplicativos Móveis.**

---

## Fim do Documento

**HortPay — Gestão agrícola e financeira para produtores rurais.**

**Última atualização: 14 de setembro de 2026**
