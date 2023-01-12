# Ejemplo 2

Ejemplo sencillo de creación de un grupo de seguridad y una instancia EC2.

La plantilla crea un grupo de seguridad con los puertos 22, 80 y 443 abiertos. También crea una instancia EC2 con la AMI de Ubuntu Server 22.04 y le asocia el grupo de seguridad.

## Crear el _stack_

```
aws cloudformation create-stack \
    --stack-name ejemplo-02 \
    --template-body file://ec2-sg.yaml
```

## Comprobar el estado del __stack_

```
aws cloudformation describe-stacks --stack-name ejemplo-02
```

## Eliminar el _stack_

```
aws cloudformation delete-stack --stack-name ejemplo-02
```