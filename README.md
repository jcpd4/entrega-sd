## Guía de Ejecución Rápida

Sigue estos pasos para poner en marcha la práctica.

### Paso A: Clonar el Repositorio

#### Paso 1: Clonar el Repositorio
```bash
git clone https://github.com/jcpd4/prac1-sd.git
cd tu-repo
```
#### Paso 2: Borrar y crear
Borra y crea un *ev_chargin.db* nuevo (IMPORTANTE)


### Paso B: kafka

#### Paso 1: descargar kafka_examen
descargar https://drive.google.com/file/d/1bp6_fHtfKEeaWFYsQZ6hb5u38yiN9qhE/view?usp=drive_link

#### Paso 2: descomprimirlo en C:/
```bash
tar -xzvf kafka_examen.tar.gz
```

#### Paso 3: cambiar las ip's en server.properties
ir a kafka>config>server.properties

```bash
listeners=PLAINTEXT://192.168.18.13:9092,CONTROLLER://localhost:9093
advertised.listeners=PLAINTEXT://192.168.18.13:9092,CONTROLLER://localhost:9093
```

#### Paso 4: Como administrador en powershell
```bash
[guid]::NewGuid().ToString()
```

#### Paso 5: Ejecuta esto en kafka
```bash
.\bin\windows\kafka-storage.bat format -t TU_UUID_AQUI -c .\config\server.properties
```

#### Paso 6: Clonar el Repositorio
```bash
.\bin\windows\kafka-server-start.bat .\config\server.properties
```

#### Paso 1: Clonar el Repositorio
#### Paso 1: Clonar el Repositorio


### Paso C: Ejecutar en PC's del aula

#### Paso 1: java
#### Paso 2: python
#### Paso 3: kafka