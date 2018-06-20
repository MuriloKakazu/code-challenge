# Desafio Salesforce

## Sobre o desafio


O tempo estimado para realizar o teste é de **uma semana e meia**, porém dependendo da sua experiência, você pode precisar de mais ou de menos tempo para realizar o desafio.

Para isso, vamos fornecer para você alguns dados. Neste site [Via CEP](https://viacep.com.br/) você é capaz de realizar uma consulta de endereços por CEP 
no formato de **{8}** dígitos, por exemplo: "01001000".

Após o CEP, deve ser fornecido o tipo de retorno desejado, que pode ser *"json"*, *"xml"*, *"piped"* ou *"querty"*.
Para realização do teste deve ser escolhido o formato *JSON*.

Exemplo de pesquisa por CEP:

```
https://viacep.com.br/ws/01415001/json/
```

Retorno da busca:

```javascript
{
  "cep": "01415-001",
  "logradouro": "Rua Bela Cintra",
  "complemento": "até 585 - lado ímpar",
  "bairro": "Consolação",
  "localidade": "São Paulo",
  "uf": "SP",
  "unidade": "",
  "ibge": "3550308",
  "gia": "1004"
}
```

## Desafio

Usando as informações anteriores, crie um lightning component que execute as seguintes funções:

### 1. Consulte um CEP e exiba para o usuário  :)

Por meio da API de consulta de CEP mencionada acima, a proposta inicial é estruturar um lightning component que
exiba as informações de endereço dado um determinado CEP que o usuário irá inputar na tela.


### 2. Gravar o endereço consultado na Conta :D

O lightning component irá conter um botão para salvar o endereço, que ao ser acionado irá gravar as informações 
consultadas pela API de CEP dentro da sessão de endereço de uma Conta.

![account_address_session](public/images/accounts-address-session.png)


## Modo de avaliação

Nós sempre avaliamos o seu código, e para isso nós envolvemos sempre no mínimo 2 engenheiros aqui do Viva e amigavelmente informamos que iremos nos basear pelos seguintes critérios:

* **Manutenibilidade:** O código é legível e de fácil manutenção?
* **Desenho:** Como foram separadas as responsabilidades? Quais técnicas foram utilizadas?
* **Qualidade:** Tem testes? Quão difícil é recriar os testes caso seja necessário alterar o comportamento da aplicação?
* **Desempenho:** Escreveu um código com performance adequada? Não precisa ser perfeito, mas entende como seria a melhor solução?

Fique a vontade para incrementar seu desafio de modo a demonstrar como o resultado do seu esforço pode deixá-lo ainda melhor!

Bom código! ;)
