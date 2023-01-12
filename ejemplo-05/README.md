# Ejemplo 5

Ejemplo sencillo de una plantilla con parámetros para crear una instancia EC2.

## Crear el _stack_

```
aws cloudformation create-stack \
  --stack-name ejemplo-05 \
  --template-body file://ejemplo-05/ec2.yaml \
  --parameters ParameterKey=KeyName,ParameterValue=vockey \
               ParameterKey=InstanceType,ParameterValue=t2.small \
               ParameterKey=ImageId,ParameterValue=ami-08e637cea2f053dfa
```

## Comprobar el estado del __stack_

```
aws cloudformation describe-stacks --stack-name ejemplo-05
```

## Eliminar el _stack_

```
aws cloudformation delete-stack --stack-name ejemplo-05
```