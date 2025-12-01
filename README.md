# Libft (42 Project) — Mandatory + Bonus

## 📘 Overview

**Libft** é o primeiro projeto da 42 e consiste em recriar funções essenciais da linguagem C,  
criando uma biblioteca própria reutilizável em futuros projetos.

Esta versão inclui **a parte obrigatória** e **os bônus**, conforme solicitado pelo subject.

---

## 🧱 Estrutura da Biblioteca

A biblioteca implementa:

- Funções de manipulação de strings
- Funções de manipulação de memória
- Funções de manipulação de caracteres
- Funções auxiliares (conversão, busca, comparação)
- Funções de listas encadeadas (bônus)
- Implementação de `ft_split`, `ft_itoa`, `ft_substr`, etc.
- Funções que replicam comportamentos da libc, respeitando todas as restrições da 42

---

## 📦 Funções da Parte Obrigatória

### 🔹 Parte 1 — Funções da libc
Todas reimplementadas seguindo comportamento idêntico:

- `ft_isalpha`, `ft_isdigit`, `ft_isalnum`, `ft_isascii`, `ft_isprint`
- `ft_strlen`, `ft_memset`, `ft_bzero`, `ft_memcpy`, `ft_memmove`
- `ft_strlcpy`, `ft_strlcat`
- `ft_toupper`, `ft_tolower`
- `ft_strchr`, `ft_strrchr`, `ft_strncmp`
- `ft_memchr`, `ft_memcmp`
- `ft_strnstr`
- `ft_atoi`
- `ft_calloc`, `ft_strdup`

### 🔹 Parte 2 — Funções adicionais
Funções utilitárias para manipulação de strings, números e memória:

- `ft_substr`
- `ft_strjoin`
- `ft_strtrim`
- `ft_split`
- `ft_itoa`
- `ft_strmapi`
- `ft_striteri`
- `ft_putchar_fd`
- `ft_putstr_fd`
- `ft_putendl_fd`
- `ft_putnbr_fd`

---

## ⭐ Bonus

### 🧩 Listas encadeadas (t_list)

Implementação completa de uma **linked list** genérica:

- `ft_lstnew`
- `ft_lstadd_front`
- `ft_lstsize`
- `ft_lstlast`
- `ft_lstadd_back`
- `ft_lstdelone`
- `ft_lstclear`
- `ft_lstiter`
- `ft_lstmap`

### 🎁 Funcionamento

As funções permitem criar, inserir, remover, iterar e transformar listas encadeadas  
de maneira genérica, utilizando ponteiros para dados e para funções.

---

## 🛠️ Compilação

Compile a biblioteca:

```bash
make
Incluindo bônus:

bash
Copiar código
make bonus
Limpar arquivos:

bash
Copiar código
make clean
make fclean
make re
O comando make gera:

Copiar código
libft.a
que pode ser incluída em qualquer projeto C.

📚 Como usar
No seu código C:

c
Copiar código
#include "libft.h"

int main(void)
{
    char *s = ft_strdup("Hello Libft!");
    ft_putendl_fd(s, 1);
    free(s);
}
Compilação:

bash
Copiar código
gcc main.c -L. -lft
🎯 O que este projeto demonstra
Conhecimento sólido de C

Entendimento profundo de alocação dinâmica

Implementação de funções da libc

Habilidade com ponteiros e manipulação de memória

Capacidade de criar e gerenciar listas encadeadas

Escrita de código limpo seguindo a Norminette

Organização modular de biblioteca

📄 Licença
Projeto acadêmico desenvolvido como parte do currículo da 42.
Livre para consulta e estudo.

yaml
Copiar código
