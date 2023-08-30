# Cert_Scraping
Web Scraping from https://stats.cert.br/incidentes/

##1. URL API

Ao Realizar o get da página para a coleta e tratativa dos dados, foi constatado que a plotagem feita no frontend é gerado em tempo de execução, puxando as informações de uma API utilizada pelo Site.
Foi constatado através do arquivo fonte da página, métodos que definem o caminho para cada API. Com tal informação, foi feita a depuração e coleta de cada uma das URLs à mão, obtendo assim as seguintes urls de conexão:

https://stats.cert.br/data/incidentes/${ano}/tipos-incidente-mensal.txt
https://stats.cert.br/data/incidentes/incidentes.txt
https://stats.cert.br/data/incidentes/dos.txt
https://stats.cert.br/data/incidentes/${ano}/tipos-incidente.txt
https://stats.cert.br/data/incidentes/${ano}/top-portas.txt
https://stats.cert.br/data/incidentes/${ano}/tipos-fraude-mensal.txt
https://stats.cert.br/data/incidentes/${ano}/incidentes-mensal.txt
https://stats.cert.br/data/incidentes/${ano}/top-cc.txt
https://stats.cert.br/data/incidentes/${ano}/top-asn.txt

onde ${ano} representa um parâmetro do tipo ano, para a obtenção das informações.
