# bandas1album - Docker

Copie o bloco de código abaixo e cole num terminal dentro de sua pasta de jobs

```shell
echo -e "\033[1;92m Clonando repositório com recurse-submodules...\033[m" &&\
git clone git@github.com:bandas1album/bandas1album-docker.git --recurse-submodules &&\
echo -e "\033[1;92m Entrando na pasta do repositório clonado...\033[m" &&\
cd bandas1album-docker &&\
echo -e "\033[1;92m Entrando na pasta docker...\033[m" &&\
cd docker &&\
echo -e "\033[1;92m Buildando o docker...\033[m" &&\
docker-compose build &&\
echo -e -e "\033[1;92m Parando possíveis dockers abertos...\033[m" &&\
dockerstop &&\
echo -e "\033[1;92m Ligando o docker...\033[m" &&\
dockerup
```
