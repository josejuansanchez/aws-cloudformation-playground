# Ejemplo 4

Ejemplo sencillo de creación de un grupo de seguridad, una instancia EC2 y una IP elástica. La IP elástica se asocia con el recurso `AWS::EC2::EIP`.

## Crear el _stack_

```
aws cloudformation create-stack \
    --stack-name ejemplo-04 \
    --template-body file://ec2-sg-eip.yaml
```

## Comprobar el estado del __stack_

```
aws cloudformation describe-stacks --stack-name ejemplo-04
```

## Eliminar el _stack_

```
aws cloudformation delete-stack --stack-name ejemplo-04
```