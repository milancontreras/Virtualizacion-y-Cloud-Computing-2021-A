## 1.Creación de la instancia EC2

La instancia EC2 serviara para  poder implementar nuestro servidor, ella pondremos nuestra página web que estara sobre el
cms wordpress. Sin emabargo para ello neceistamos configurar ciertos servicios primeros como lo es  WAF (firewall), los grupos de seguridad y el par de clases para poder conectarnos a nuestra instancia.

1. In the AWS Management Console choose **Services** then select **S3** under Storage.

1. Choose **Create Bucket**

1. Provide a globally unique name for your bucket such as `vod-watchfolder-firstname-lastname`.

1. Select the Region you've chosen to use for this workshop from the dropdown.

1. Choose **Create** in the lower left of the dialog without selecting a bucket to copy settings from.

    ![Create source bucket screenshot](../images/s3-create-watchfolder.png)

