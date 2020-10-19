Arquivos de configuração para telefone CISCO IP 7942/7962G para conexão ao SIP.

- O arquivo SEPMAC.cnf.xml deve ser renomeado, substituindo MAC pelo endereço MAC do telefone.

<b>Informações a alterar no arquivo modelo:</b>

- Configurações de data e hora:

Formado a ser exibido a data e hora:
<dateTemplate>D-M-YY</dateTemplate>

Zona horária
<timeZone>America/Sao_Paulo</timeZone>

Servidor NTP
<ntps>
    <ntp>
		<name>IP DO SERVIDOR</name>
		<ntpMode>Unicast</ntpMode>
	</ntp>
</ntps>

- Configurações de portas SIP

<ethernetPhonePort>2000</ethernetPhonePort>
<sipPort>5060</sipPort>
<securedSipPort>5061</securedSipPort>
<processNodeName>IP PABX</processNodeName>


- Configurações do ramal

<featureLabel>RAMAL</featureLabel>
<port>5060</port>
<name>RAMAL</name>
<displayName>RAMAL</displayName> #nome a ser exibido na tela do aparelho
<authName>RAMAL</authName>
<authPassword>SENHA RAMAL</authPassword>
<messagesNumber>*97</messagesNumber> #número do correio de voz

