# Ejemplo 1

Ejemplo sencillo de creación de una instancia EC2.

## Crear el _stack_

```
aws cloudformation create-stack \
    --stack-name ejemplo-01 \
    --template-body file://ec2.yaml
```

## Comprobar el estado del __stack_

```
aws cloudformation describe-stacks --stack-name ejemplo-01
```

## Eliminar el _stack_

```
aws cloudformation delete-stack --stack-name ejemplo-01
```