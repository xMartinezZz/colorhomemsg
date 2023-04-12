# Color Home Message
Aplicação criada para praticar conceitos de Kubernetes e Helm Chats para efetuar o deploy de aplicações 
em ambientes kubernetes com controle imagens pelo helm

Para executar a imagem docker primeiro faça o build da imagem
```dockerfile
docker build -t xmartinezzz/colorhomemsg:latest .
```

Em seguida execute a imagem passando os parâmetros como variáveis de ambiente

TEXT -> Mensagem que aparecerá na tela

COLOR -> Cor de fundo aplicada ao css
```bash
docker run --rm -d -p 8080:8080 -e "TEXT=MENSAGEM TESTE" -e 'COLOR="BLUE"' --name colormsg xmartinezzz/colorhomemsg

```

TODO:
- [ ] Inserir passo a passo para reprodução
- [ ] Inserir descrição mais detalhada