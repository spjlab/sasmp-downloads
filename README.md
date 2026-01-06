# SASMP
### Sistema de Automação de Serviços de Multa Penal

![Badge](https://img.shields.io/badge/status-stable-green) ![Platform](https://img.shields.io/badge/platform-macOS%20%7C%20Windows-lightgrey) ![Release](https://img.shields.io/github/v/release/spjlab/sasmp-downloads?label=latest)

---

## Sobre o Projeto

O **SASMP (Sistema de Automação de Serviços de Multa Penal)** é uma solução de software de nível corporativo desenvolvida para automatizar, gerenciar e otimizar o fluxo de trabalho relacionado às certidões de penas de multa no âmbito do Ministério Público do Estado de São Paulo.

Este repositório atua como o **canal de distribuição** das compilações (releases) públicas da aplicação. O código-fonte principal é mantido em um repositório privado para garantir a integridade e segurança das regras de negócio proprietárias.

> **Nota:** Este software foi projetado com arquitetura focada em **segurança**, **privacidade de dados** (Offline-First) e **alta performance**.

---

## Destaques Técnicos

Embora a interface seja amigável e intuitiva, o SASMP opera sobre uma engenharia robusta:

- **Arquitetura Híbrida Moderna**: Construído sobre **Electron** e **Next.js**, unindo a segurança do desktop com a reatividade da web moderna.
- **Offline-First com SQLite**: Persistência de dados local extremamente rápida e segura, sem dependência constante de conexão com a internet.
- **Automação Inteligente**: Integração com **Playwright** para automação de tarefas repetitivas nos portais institucionais.
- **Processamento de Documentos**: Pipeline nativo para leitura, OCR (Tesseract) e manipulação de PDFs.
- **Segurança**: Implementação rigorosa de **Context Isolation**, **CSP (Content Security Policy)** e sanitização de inputs.

---

## Instalação e Downloads

As versões mais recentes para **macOS** (Apple Silicon/Intel) e **Windows** estão disponíveis na aba **[Releases](/spjlab/sasmp-downloads/releases)** deste repositório.

### macOS
1. Baixe o instalador `.pkg` (Recomendado) ou `.dmg`.
2. Para instalar o `.pkg`, clique com o **Botão Direito > Abrir** para autorizar a execução.

### Windows
1. Baixe o instalador `.exe`.
2. Execute o instalador (instalação automática no perfil do usuário, sem necessidade de privilégios de administrador).

3. > [!NOTE]
> **Aviso de Transparência (SmartScreen / Gatekeeper)**
>
> Como este software é uma iniciativa independente e sem fins comerciais, ele não utiliza certificados digitais de alto custo (EV Code Signing). Por isso, o Windows ou macOS podem exibir alertas de "Fornecedor Desconhecido" ou "Proteção do PC" na primeira execução.
>
> **Isso é um comportamento padrão para softwares que não são distribuídos via App Store.** Para prosseguir:
> - **Windows**: Clique em *"Mais informações"* e depois em *"Executar assim mesmo"*.
> - **macOS**: Clique com o botão direito no instalador e selecione *"Abrir"*.
>   - *Se não funcionar:* Vá em **Ajustes do Sistema > Privacidade e Segurança**, role até o fim e clique em **"Abrir Mesmo Assim"**.

---

## Stack Tecnológica

O desenvolvimento do SASMP utiliza as melhores práticas de Engenharia de Software atuais:

| Categoria | Tecnologias |
| :--- | :--- |
| **Core** | TypeScript, React, Electron |
| **Frontend** | Next.js (App Router) |
| **Main Process** | Electron IPC (Seguro e Nativo) |
| **UI/UX** | TailwindCSS, Shadcn/ui |
| **Base de Dados** | Kysely Query Builder, Better-SQLite3 |
| **Automação** | Playwright |
| **CI/CD** | GitHub Actions (Automated Cross-Platform Builds) |

---

## Contato e Suporte

Para suporte técnico, reporte de bugs ou solicitações de funcionalidades, encaminhe um e-mail para [sergio@pereirajunior.org](mailto:sergio@pereirajunior.org).

---

&copy; 2025-2026 **Sergio Pereira Junior**. Todos os direitos reservados.

🌐 [pereirajunior.org](https://pereirajunior.org)
