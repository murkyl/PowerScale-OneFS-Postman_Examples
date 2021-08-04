# PowerScale/OneFS Postman Examples
This repository holds examples of the API commands for [PowerScale/OneFS](https://www.delltechnologies.com/en-us/storage/powerscale.htm) using Postman.

When you import the collection into your Postman instance, you also need to import the environment variables. You will then need to fill out the current values for most of the variables to have the collections working in the way they have been designed.

Below is a table explaining each required variable field and what type of values are needed.

# Required environment variable settings
| Variables    | Description                                                             |
| ------------ | ----------------------------------------------------------------------- |
| username     | Provide a user with sufficient RBAC privileges                          |
| password     | Password for the user specified in 'username'                           |
| endpoint     | The full URL with FQDN or IP address and port of the PowerScale cluster |
| api_version  | API version to use. See below table for the OneFS to API version matrix |

The API version will differ depending on the version of OneFS you want to communicate with. The following table defines the API version and OneFS version matrix.

|   API Version   | --- |   OneFS Version   |
|:---------------:|-----|:-----------------:|
|        1        |     |      7.2.0.0      |
|        2        |     |      7.2.1.0      |
|        3        |     |      8.0.0.0      |
|        4        |     |      8.0.1.0      |
|        5        |     |      8.1.0.0      |
|        6        |     |      8.1.1.0      |
|        7        |     |      8.2.0.0      |
|        8        |     |      8.2.1.0      |
|        9        |     |      8.2.2.0      |
|        10       |     |      9.0.0.0      |
|        11       |     |      9.1.0.0      |
|        12       |     |      9.2.0.0      |

When working with the S3 API calls, additional environment variables need to be configured.

| Variables        | Description                                                             |
| ---------------- | ----------------------------------------------------------------------- |
| s3_endpoint      | The full URL with FQDN or IP address and port of the PowerScale cluster |
| s3_access_id     | S3 account ID that is created on the PowerScale cluster				 |
| s3_access_secret | S3 account secret that is created on the PowerScale cluster             |

The s3_endpoint value should be in one of 2 forms: http://fqdn_or_ip:9020 or https://fqdn_or_ip:9021