# WeSender SDK para C#
  SDK para conexão com a API em C#

**A chave da api deve ser passada na instância da classe, como construtor**

`Install-Package WeSenderSDK`

## Métodos diponiveis no momento
### - sendMessage
Esse metodo recebe `três parametros` com as informações que devem ser enviadas e para quem deve ser enviado.
 ```cs
SendMessage (List<string> destines, string message, bool hasSpecialCharacter = false)
 ``` 
Resposta do método é a mesma que a da API:
```cs

{
  "Success" : bool,
  "Message" : String,
}

```

## Exemplo

```cs
using WeSenderSDK;
var WSDK = new WeSender("apikey");
var destines = new List<string>();
destines.Add("920000000");
var response = WSDK.SendMessage(destines, "Olá Angola");
```

## 🤔 Como contribuir

- Faça um fork desse repositório;
- Cria uma branch com a sua feature: `git checkout -b minha-feature`;
- Faça commit das suas alterações: `git commit -m 'feat: Minha nova feature'`;
- Faça push para a sua branch: `git push origin minha-feature`.

Depois que o merge da sua pull request for feito, você pode deletar a sua branch.

## :memo: Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE.md) para mais detalhes.

## Contribuidores
[Erikson Melgarejo](mailto:mailto:erikson.melgarejo@digitalfactory.co.ao)

[Carlos Garcia](https://github.com/CarlCr)

## Autor
[Acidiney Dias](mailto:mailto:acidiney.dias@digitalfactory.co.ao)
