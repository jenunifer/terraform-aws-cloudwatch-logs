## terraform-aws-cloudwatch-logs [![Build Status](https://travis-ci.org/cloudposse/terraform-aws-cloudwatch-logs.svg?branch=master)](https://travis-ci.org/cloudposse/terraform-aws-cloudwatch-logs)
<!---
  --- This file was automatically generated by the `build-harness`
  --- Make changes instead to `.README.md` and rebuild.
  --->

Terraform module for creation of CloudWatch Log Streams and Log Groups for use with Fluentd.

## Usage

```terraform
module "cloudwatch_log" {
  namespace    = "${var.namespace}"
  stage        = "${var.stage}"
  stream_names = ["kafka-instance-1", "kafka-instance-2"]
}
```

## Input

<!--------------------------------REQUIRE POSTPROCESSING-------------------------------->
|  Name |  Default  |  Description  |
|:------|:---------:|:--------------:|
| additional_permissions |[] |Additional permissions granted to assumed role|
| attributes |[] |Additional attributes (e.g. `policy` or `role`)|
| delimiter |"-" |Delimiter to be used between `name`, `namespace`, `stage`, etc.|
| name |"" |Name  (e.g. `bastion` or `db`)|
| namespace |__REQUIRED__ |Namespace (e.g. `cp` or `cloudposse`)|
| retention_in_days |"30" |Number of days you want to retain log events in the log group|
| stage |__REQUIRED__ |Stage (e.g. `prod`, `dev`, `staging`)|
| stream_names |[] |Names of streams|
| tags |{} |Additional tags (e.g. map(`BusinessUnit`,`XYZ`)|
| trusted_roles |[] |Roles allow to assume role|

## Output

<!--------------------------------REQUIRE POSTPROCESSING-------------------------------->
|  Name | Description  |
|:------|:------------:|
| assumed_role_arn | ARN of role to assume  |
| assumed_role_name | Name of role to assume  |
| log_group_arn | ARN of the log group  |
| log_group_name | Name of log group  |
| policy_arn | ARN of role to assume  |
| policy_name | Name of role to assume  |
| stream_arns | ARN of the log stream  |

## Help

**Got a question?**

File a GitHub [issue](https://github.com/cloudposse/terraform-aws-cloudwatch-logs/issues), send us an [email](mailto:hello@cloudposse.com) or reach out to us on [Gitter](https://gitter.im/cloudposse/).

## Contributing

### Bug Reports & Feature Requests

Please use the [issue tracker](https://github.com/cloudposse/terraform-aws-cloudwatch-logs/issues) to report any bugs or file feature requests.

### Developing

If you are interested in being a contributor and want to get involved in developing `terraform-aws-cloudwatch-logs`, we would love to hear from you! Shoot us an [email](mailto:hello@cloudposse.com).

In general, PRs are welcome. We follow the typical "fork-and-pull" Git workflow.

 1. **Fork** the repo on GitHub
 2. **Clone** the project to your own machine
 3. **Commit** changes to your own branch
 4. **Push** your work back up to your fork
 5. Submit a **Pull request** so that we can review your changes

**NOTE:** Be sure to merge the latest from "upstream" before making a pull request!

## License

[APACHE 2.0](LICENSE) © 2017 [Cloud Posse, LLC](https://cloudposse.com)

See [LICENSE](LICENSE) for full details.

    Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
    with the License.  You may obtain a copy of the License at

      http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing,
    software distributed under the License is distributed on an
    "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.

## About

This project is maintained and funded by [Cloud Posse, LLC][website]. Like it? Please let us know at <hello@cloudposse.com>

We love [Open Source Software](https://github.com/cloudposse/)!

See [our other projects][community]
or [hire us][hire] to help build your next cloud-platform.

  [website]: http://cloudposse.com/
  [community]: https://github.com/cloudposse/
  [hire]: http://cloudposse.com/contact/

### Contributors

|[![Erik Osterman][erik_img]][erik_web]<br/>[Erik Osterman][erik_web] |[![Vladimir][vladimir_img]][vladimir_web]<br/>[Vladimir][vladimir_web] |[![Igor Rodionov][igor_img]][igor_web]<br/>[Igor Rodionov][igor_img] |
|---|---|---|

[andriy_img]: https://avatars0.githubusercontent.com/u/7356997?v=4&u=ed9ce1c9151d552d985bdf5546772e14ef7ab617&s=144
[andriy_web]: https://github.com/aknysh/

[erik_img]: http://s.gravatar.com/avatar/88c480d4f73b813904e00a5695a454cb?s=144
[erik_web]: https://github.com/osterman/

[igor_img]: http://s.gravatar.com/avatar/bc70834d32ed4517568a1feb0b9be7e2?s=144
[igor_web]: https://github.com/goruha/

[konstantin_img]: https://avatars1.githubusercontent.com/u/11299538?v=4&u=ed9ce1c9151d552d985bdf5546772e14ef7ab617&s=144
[konstantin_web]: https://github.com/comeanother/

[sergey_img]: https://avatars1.githubusercontent.com/u/1134449?v=4&u=ed9ce1c9151d552d985bdf5546772e14ef7ab617&s=144
[sergey_web]: https://github.com/s2504s/

[valeriy_img]: https://avatars1.githubusercontent.com/u/10601658?v=4&u=ed9ce1c9151d552d985bdf5546772e14ef7ab617&s=144
[valeriy_web]: https://github.com/drama17/

[vladimir_img]: https://avatars1.githubusercontent.com/u/26582191?v=4&u=ed9ce1c9151d552d985bdf5546772e14ef7ab617&s=144
[vladimir_web]: https://github.com/SweetOps/
