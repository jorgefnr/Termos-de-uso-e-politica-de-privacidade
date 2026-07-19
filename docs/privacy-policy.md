---
layout: default
title: Política de Privacidade - HortPay
---

# Política de Privacidade — HortPay

**Última atualização:** 18 de julho de 2026

Esta Política de Privacidade descreve como o aplicativo **HortPay** (referido como "app", "nós" ou "HortPay") coleta, utiliza, armazena e protege as informações fornecidas por você, o usuário. Ao usar o HortPay, você concorda com as práticas descritas nesta política.

---

## 1. Quem somos

O HortPay é um aplicativo móvel de gestão financeira agrícola voltado para pequenos e médios produtores rurais. Nosso objetivo é facilitar o controle de vendas, produtos, ciclos de cultivo, análises de solo e fluxo de caixa, com armazenamento **local no dispositivo do usuário** e opção de backup automático na nuvem via Google Drive.

Contato: gestaodeestufashf@gmail.com

---

## 2. Dados que coletamos

### 2.1. Dados criados por você no app (armazenados localmente)

O HortPay armazena, **exclusivamente no banco de dados SQLite local do seu dispositivo**, os seguintes tipos de informação:

- Cadastros de estufas, produtos, ciclos de cultivo, aplicações e insumos
- Registros de vendas, compradores, valores, datas e formas de pagamento
- Movimentações financeiras (entradas, saídas, transferências)
- Cartões de crédito registrados (**apenas apelido escolhido por você e últimos 4 dígitos** — nunca o número completo, CVV ou senha)
- Parcelas de compras e contas a pagar
- Custos de cultivo, análises de solo (resultados numéricos)
- Configurações do aplicativo, preferências, tema, moeda

**Não coletamos**: nome completo do usuário, CPF, endereço residencial, telefone, senhas bancárias, imagem de documentos, dados biométricos ou qualquer informação de identificação pessoal sensível.

### 2.2. Dados enviados para o Google Drive (backup na nuvem, opcional)

Se você optar por usar o recurso de **Backup na Nuvem**, uma cópia dos dados do item 2.1 é enviada em formato JSON para uma pasta oculta da sua própria conta Google Drive, chamada **AppDataFolder**. Esta pasta:

- É invisível para você na interface do Google Drive
- É acessível **apenas** pelo aplicativo HortPay que criou os arquivos
- **NÃO pode ser acessada** por outros aplicativos, mesmo que você tenha instalado outros apps que usem Google Drive
- Fica na sua própria conta Google — o HortPay não mantém cópia em servidores próprios

### 2.3. Dados fornecidos pelo Google no login (Google Sign-In)

Quando você conecta sua conta Google para ativar o backup na nuvem, o Google nos fornece:

- **Seu endereço de email** (usado para identificar sua conta)
- **Seu nome público** (mostrado na tela de backup)
- **Foto do perfil** (opcional, mostrada na tela de backup)

Essas informações ficam armazenadas apenas no seu dispositivo, no SecureStore (armazenamento criptografado por hardware) do Android/iOS. Não enviamos essas informações para servidores nossos ou de terceiros.

### 2.4. Tokens de acesso ao Google Drive

Após o consentimento, o Google nos fornece dois tokens:

- **Access token** (curto prazo, ~1 hora) — usado para chamadas à API do Drive
- **Refresh token** (longo prazo, até você revogar) — usado para renovar o access token automaticamente

Ambos os tokens são armazenados no **SecureStore** (Android Keystore / iOS Keychain), com criptografia baseada em hardware. Mesmo com acesso físico ao aparelho, extrair esses tokens é impraticável sem root/jailbreak.

---

## 3. Como usamos os dados

- Os dados armazenados localmente (2.1) são usados **exclusivamente** para exibir suas informações no próprio app (relatórios, gráficos, listas).
- Os dados enviados ao Drive (2.2) são usados **exclusivamente** para permitir que você recupere seus dados caso troque, perca ou danifique o dispositivo.
- Os dados do Google (2.3, 2.4) são usados **exclusivamente** para autenticação e comunicação com a API do Google Drive.

**NÃO fazemos**:

- ❌ Análise de comportamento, tracking, publicidade direcionada
- ❌ Compartilhamento com terceiros
- ❌ Venda de dados
- ❌ Envio de emails de marketing
- ❌ Coleta de estatísticas anônimas em servidores próprios

---

## 4. Onde os dados ficam armazenados

| Tipo de dado | Local |
|---|---|
| Dados cadastrados no app (produtos, vendas, etc) | Banco SQLite local no seu dispositivo |
| Backup na nuvem | Google Drive AppDataFolder da sua própria conta Google |
| Tokens OAuth | SecureStore (criptografia por hardware) do seu dispositivo |
| Preferências e configurações | AsyncStorage local do seu dispositivo |

**Não temos servidores próprios armazenando qualquer dado seu.** Todo o processamento acontece no seu dispositivo e/ou diretamente entre seu dispositivo e a API do Google.

---

## 5. Segurança

- Tokens OAuth armazenados no SecureStore (criptografia por hardware — Android Keystore / iOS Keychain)
- Autenticação OAuth 2.0 com PKCE (Proof Key for Code Exchange) — padrão do setor
- Comunicação com API do Google via HTTPS/TLS 1.2+ (garantido pelo Google)
- Escopo restrito ao AppDataFolder — o app NÃO tem permissão para ler outros arquivos do seu Drive
- Import de backup usa transaction SQLite (rollback automático em caso de falha, impedindo estados corrompidos)
- Snapshot automático de segurança criado antes de qualquer restauração de backup

---

## 6. Seus direitos

Você pode, a qualquer momento:

1. **Fazer backup manual** — Configurações → Backup na Nuvem → "Fazer backup agora"
2. **Restaurar um backup** — Tocando em qualquer backup listado na tela
3. **Desativar backup automático** — Configurações → Backup na Nuvem → Switch "Backup automático"
4. **Desconectar sua conta Google** — Configurações → Backup na Nuvem → Botão "Desconectar conta Google"
5. **Revogar completamente o acesso do HortPay ao seu Drive** — em [myaccount.google.com/security](https://myaccount.google.com/security) → "Apps de terceiros com acesso à conta" → HortPay → Remover acesso
6. **Excluir todos os backups** — solicitar via email `hortpay.suporte@gmail.com` OU deletar manualmente na tela de Backup na Nuvem (função "Deletar todos" na versão de debug)
7. **Excluir dados locais** — Configurações do sistema do Android → Aplicativos → HortPay → Armazenamento → "Limpar dados"

---

## 7. Retenção de dados

- **Backups na nuvem**: mantemos até 5 backups automáticos por conta (rotação). Backups mais antigos são excluídos automaticamente. Você pode excluir a qualquer momento.
- **Dados locais**: permanecem enquanto o app estiver instalado. Ao desinstalar, todos os dados locais são removidos.
- **Tokens OAuth**: mantidos enquanto você não revogar. Você pode revogar a qualquer momento.

---

## 8. Compartilhamento de dados com terceiros

**Nenhum dado é compartilhado com terceiros**, exceto:

- **Google LLC** — para autenticação e armazenamento do backup na sua conta Google Drive (regido pela [Política de Privacidade do Google](https://policies.google.com/privacy))

Não há SDKs de analytics, tracking, ads ou crash reporting de terceiros no aplicativo.

---

## 9. Menores de idade

O HortPay é destinado a produtores rurais maiores de 18 anos. Não coletamos intencionalmente dados de menores de idade. Se você é responsável por um menor e acredita que ele forneceu informações ao app, entre em contato para removermos.

---

## 10. Alterações nesta política

Podemos atualizar esta política a qualquer momento. A data de "Última atualização" no topo da página será alterada. Uso continuado do app após uma atualização implica aceitação da política revisada. Alterações significativas serão notificadas via update do aplicativo.

---

## 11. Contato

Dúvidas, solicitações de exclusão de dados ou reclamações:

**Email:** gestaodeestufashf@gmail.com

---

*HortPay © 2026. Aplicativo desenvolvido de forma independente. Não afiliado ou endossado pelo Google LLC.*
