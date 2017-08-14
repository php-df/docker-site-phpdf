# PHPDF Site - Docker

[English Version](./README-EN.md)

Agora é possível ter toda a Stack do novo site do PHPDF diretamente em sua máquina, possibilitando o acompanhamento, envio de sugestões e melhorias.

### Sobre

As soluções de proxy reverso desse repositório foram fornecidas pelo repo [devbrotherhood/docker-reverse-proxy](https://github.com/devbrotherhood/docker-reverse-proxy) e são usadas para vincular vários domínios em aplicativos específicos de porta para docker, permitindo que múltiplos contêineres sejam executados em diferentes portas, mas respondendo a uma porta padrão como 80 por exemplo.

### Como usar

Nesta solução, usamos a ferramenta "docker-compose" do Docker. Para fazer este trabalho.
 
Vamos aos passos:

- Adicione seu host em `/etc/hosts`
- Duplique os arquivos `docker-compose.yml_sample` e `./conf/my_proxy.conf_sample` respectivamente para `docker-compose.yml` e `conf/my_proxy.conf` ajustando de acordo com sua necessidade.  
- Execute o comando abaixo para que o docker levante toda a stack da sua aplicação:

```
     docker-compose up
```

### Referências

- https://github.com/devbrotherhood/docker-reverse-proxy
