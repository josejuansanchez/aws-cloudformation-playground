# aws-cloudformation-playground

Repositorio para hacer experimentos con AWS CloudFormation.

- [Ejemplo 01](ejemplo-01/ec2.yaml). Creación de una instancia EC2.
- [Ejemplo 02](ejemplo-02/ec2-sg.yaml). Creación de un grupo de seguridad y una instancia EC2.
- [Ejemplo 03](ejemplo-03/ec2-sg-eip.yaml). Creación de un grupo de seguridad, una instancia EC2 y una IP elástica. La IP elástica se asocia con el recurso `AWS::EC2::EIPAssociation`.
- [Ejemplo 04](ejemplo-04/ec2-sg-eip.yaml). Creación de un grupo de seguridad, una instancia EC2 y una IP elástica. La IP elástica se asocia con el recurso `AWS::EC2::EIP`.
- [Ejemplo 05](ejemplo-05/ec2.yaml). Plantilla con parámetros para crear una instancia EC2.