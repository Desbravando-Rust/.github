# Desbravando Rust

**Um guia prático para pythonistas explorarem novos horizontes**

[![Comprar Livro](https://img.shields.io/badge/Comprar-R$_89,90-orange?style=for-the-badge)](https://desbravandorust.com.br)
[![Site Oficial](https://img.shields.io/badge/Site_Oficial-desbravandorust.com.br-blue?style=for-the-badge)](https://desbravandorust.com.br)

---

## Sobre o Livro

<img src="imgs/capa.jpg" alt="Capa do Livro Desbravando Rust" width="120" align="left">

**Desbravando Rust** é um guia técnico completo desenvolvido especialmente para desenvolvedores Python que desejam expandir suas habilidades para uma linguagem de alto desempenho e segurança: Rust.

Este livro oferece uma transição didática e prática, comparando conceitos, sintaxes e melhores práticas entre Python e Rust, permitindo que você aproveite seu conhecimento existente enquanto domina uma das linguagens mais admiradas da atualidade.

Se você busca otimizar performance, explorar concorrência de forma segura ou simplesmente ampliar seu conjunto de habilidades técnicas, este livro foi feito para você.


## Para Quem é Este Livro

- Desenvolvedores Python que desejam aprender Rust de forma prática e comparativa
- Engenheiros de software buscando melhorar performance e segurança de aplicações
- Profissionais interessados em sistemas concorrentes e paralelismo
- Desenvolvedores que querem expandir seu portfólio técnico com uma linguagem moderna
- Programadores que trabalham com infraestrutura crítica e precisam de garantias de segurança de memória

## O Que Você Vai Aprender

### Fundamentos da Linguagem

**Sintaxe e Estruturas de Dados**
- Comparação direta entre Python e Rust
- Constantes, variáveis e mutabilidade explícita
- Tipos de dados primitivos e compostos
- Pattern matching e controle de fluxo

**Gerenciamento de Memória**
- Ownership (propriedade): o coração da segurança de Rust
- Borrowing (empréstimo): referências seguras e eficientes
- Lifetimes: garantias de validade de referências em tempo de compilação
- Stack vs Heap: otimização de alocação de memória

**Tratamento de Erros**
- Result e Option: tipos para tratamento robusto de erros
- Comparação com try/except do Python
- Propagação de erros idiomática com o operador `?`
- Panic e recovery: quando e como usá-los

### Tópicos Avançados

**Concorrência e Paralelismo**
- Threads seguras: modelo de ownership previne data races
- Channels para comunicação entre threads
- Async/await para operações assíncronas
- Mutexes e sincronização segura

**Ecossistema e Ferramentas**
- Cargo: gerenciador de pacotes e build system
- Crates: bibliotecas do ecossistema Rust
- Testing integrado e documentação automática
- Benchmarking e profiling de performance

## Projetos Práticos

O livro inclui implementações completas de projetos reais, do básico ao avançado:

### 1. Concatenador de Arquivos
Aplicação CLI para processamento de arquivos, demonstrando manipulação de I/O e tratamento de erros.

### 2. API REST de Agendamento
Sistema completo de agendamento usando **Axum**, incluindo:
- Roteamento e handlers HTTP
- Integração com PostgreSQL
- Middleware e autenticação
- Validação de dados e error handling

### 3. Autenticação TOTP com AWS Lambda
Implementação de Two-Factor Authentication (2FA) serverless:
- Geração e validação de tokens TOTP
- Deploy em AWS Lambda
- Integração com serviços cloud
- Arquitetura serverless com Rust

## Performance: Rust vs Python

O livro demonstra, através de benchmarks reais, as diferenças de performance entre as linguagens:


```rust
// Exemplo: Cálculo de Fatorial em Rust
use std::time::Instant;

fn factorial(n: u64) -> u64 {
    let mut result = 1;
    for i in 1..=n {
        result *= i;
    }
    result
}

fn main() {
    let n: u64 = 10;
    let start = Instant::now();
    let result = factorial(n);
    let duration = start.elapsed();

    println!("Fatorial de {} = {}", n, result);
    println!("Tempo de execução em Rust: {:?}", duration);
}
```
Output: Tempo de execução em Rust: 495ns


```python
# Mesmo exemplo em Python
import time

def factorial(n: int) -> int:
    result = 1
    for i in range(1, n + 1):
        result *= i
    return result

if name == "main":
    n = 10
    start = time.time()
    result = factorial(n)
    end = time.time()

    print(f"Fatorial de {n} = {result}")
    print(f"Tempo de execução em Python: {end - start:.6f} segundos")
```
Output: Tempo de execução em Python: 0.000006 segundos


**Resultado**: Rust foi aproximadamente **12 vezes mais rápido** neste caso específico.

## Estrutura do Conteúdo

O livro é organizado de forma progressiva, permitindo uma curva de aprendizado natural:

1. **Introdução e Setup**: Instalação e configuração do ambiente Rust
2. **Fundamentos**: Sintaxe básica, tipos e controle de fluxo
3. **Ownership e Borrowing**: O modelo de memória único do Rust
4. **Estruturas de Dados**: Vetores, strings, hashmaps e structs
5. **Traits e Generics**: Abstração e reutilização de código
6. **Tratamento de Erros**: Result, Option e error handling idiomático
7. **Coleções e Iteradores**: Processamento eficiente de dados
8. **Concorrência**: Threads, async/await e paralelismo seguro
9. **Projetos Práticos**: Aplicações completas do mundo real
10. **Deploy e Produção**: Otimização, testes e deployment

## Diferenciais do Livro

- **Abordagem Comparativa**: Cada conceito é explicado comparando com Python, facilitando a compreensão
- **Foco Prático**: Exemplos reais e projetos completos, não apenas teoria
- **Erros de Compilação Explicados**: Entenda as mensagens do compilador Rust e como resolvê-las
- **Boas Práticas**: Padrões idiomáticos e convenções da comunidade Rust
- **Progressivo**: Do Hello World até aplicações production-ready
- **Exemplos**: Código-fonte de todos os exemplos do livro
- **Em português**: Todo o livro está em português (pt-br)


## Adquira o Livro

O livro está disponível em formato **PDF digital** e pode ser adquirido através do site oficial:

**[🔗 desbravandorust.com.br](https://desbravandorust.com.br)**

**Preço**: R$ 89,90
**Entrega**: PDF em até 2 dias úteis após a compra

### O Que Você Recebe

- Livro completo em PDF com mais de 400 páginas;
- Código-fonte de todos os projetos

## Sobre o Autor

**José Luis da Cruz Junior**
Senior Software Engineer com 22+ anos de experiência em desenvolvimento backend, especializado em Python e Rust.

- [LinkedIn](https://www.linkedin.com/in/jose-luis-da-cruz-junior/)
- [GitHub](https://github.com/seu-usuario)

## Comunidade e Suporte

Tem dúvidas ou sugestões?
- **Email**: desbravandorust@gmail.com


---

<small>**XWDEV Web Solutions LTDA** | Todos os direitos reservados © 2025</small>

**Comece sua jornada em Rust hoje mesmo!**
