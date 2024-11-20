
### Controle de versão com Git
![[Pasted image 20241108142126.png|100]]

---

Imaginem que estão a trabalhar num site

![[Apresentação sobre Git e GIthub 2024-11-08 14.24.26.excalidraw|200]]

---

Mas apagam algum ficheiro importante sem querer

![[Apresentação sobre Git e GIthub 2024-11-08 14.28.13.excalidraw|200]]

---

## Como vocês acham que podemos prevenir isto?

---

## 1. Backups

![[Apresentação sobre Git e GIthub 2024-11-08 14.31.41.excalidraw|200]]

---

### Backups são ineficientes

![[Apresentação sobre Git e GIthub 2024-11-08 14.37.27.excalidraw|150]]

---

# 2. Git

![[Pasted image 20241108142126.png|200]]

---

### Como funciona?

![[Apresentação sobre Git e GIthub 2024-11-08 14.58.50.excalidraw|800]]

---
#### Comandos básicos

| Comando                           | Descrição                                         |
| --------------------------------- | ------------------------------------------------- |
| `git init`                        | Cria um **repositório**                           |
| `git add <ficheiro>`              | Seleciona um ficheiro para ser incluído no commit |
| `git commit`                      | Cria um novo commit                               |
| `git reset --hard <id do commit>` | Volta para um commit anterior                     |

---

## Lazygit

![[lazygit.mp4]]

---

## Reversão de alterações

![[lazygit reversão.mp4]]

---

#### Antes de usarem git, eu quero dizer antes uma coisa

---

### POR FAVOR ESCREVAM MENSAGENS DE COMMIT UTEIS
- ✗ “Alterações”
- ✗ “Coisas”
- ✗ “ljbrljkgbekgbeçkjb”
- ✓ “Adicionar botão de voltar na página de checkout”
- ✓ “Resolver bug que ele não carregava a página”