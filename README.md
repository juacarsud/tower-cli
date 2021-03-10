tower-cli workflow create --name="empresa1-IAC-DEV-VW-WIN2016-IIS" --organization="empresa1"
tower-cli workflow schema empresa1-IAC-DEV-VW-WIN2016-IIS @schema.yml
tower-cli workflow survey --name="empresa1-IAC-DEV-VW-WIN2016-IIS" > s.json
tower-cli workflow modify --name="empresa1-IAC-DEV-VW-WIN2016-IIS" --survey-spec=@s.json