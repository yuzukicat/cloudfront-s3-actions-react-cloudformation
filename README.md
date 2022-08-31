<div id="top"></div>

![Contributors][contributors-shield]

![Pull Request || AWS CodeCommit][pull-request-shield]

![Issues][issues-shield]

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/yuzukicat/cloudfront-s3-actions-react">
    <img src="https://eyesjapan.atlassian.net/rest/api/2/universal_avatar/view/type/project/avatar/15000?size=xxlarge&quot" alt="food-plating-ai" width="80" height="80">
  </a>

  <h3 align="center">Food Plating AI</h3>

  <p align="center">
    Front-end Development with Google Angular
    <br />
    <a href="https://github.com/yuzukicat/cloudfront-s3-actions-react"><strong>Cloudfront S3 Actions React »</strong></a>
    <br />
    <br />
    <a href="https://github.com/yuzukicat/cloudfront-s3-actions-react/issues">Report Issue</a>
    ·
    <a href="https://github.com/yuzukicat/cloudfront-s3-actions-react/pulls">Pull Request</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Git Clone</a></li>
      </ul>
    </li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

[![Food AI Site Screen Shot][product-screenshot]](/src/assets/about/about-the-project.png)

<p align="right">(<a href="#top">back to top</a>)</p>

### Built With

* [AWS CloudFormation | S3 | CloudFront](https://docs.aws.amazon.com/prescriptive-guidance/latest/patterns/deploy-a-react-based-single-page-application-to-amazon-s3-and-cloudfront.html)
* [Github Actions](https://github.com/features/actions)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

### Prerequisites

* An active AWS account.
* Bucket restrictions and limitations not excess 100. Or you may need to remove unused S3 buckets. If you need additional buckets, submit a support ticket to increase your limit. However, there is a hard limit of 1000 S3 buckets per account. See [AWS S3 | Bucket restrictions and limitations](https://docs.aws.amazon.com/AmazonS3/latest/userguide/BucketRestrictions.html)

### How To

1. Clone the repo
```sh
git clone https://github.com/yuzukicat/cloudfront-s3-actions-react
```

2. Floder Premission.
```sh
cd ..
sudo chmod -R 777 cloudfront-s3-actions-react
cd cloudfront-s3-actions-react
```

3. To Create the infrastructure to host and expose a React Single Page Application:
Deploy the AWS CloudFormation template.
See [AWS Rrescriptive Guidance | Websites & web apps](https://docs.aws.amazon.com/prescriptive-guidance/latest/patterns/deploy-a-react-based-single-page-application-to-amazon-s3-and-cloudfront.html)
- Epics
  - Deploy the SPA
    - Deploy the AWS CloudFormation template: Change the option as follow:
- Stack failure options
  - Preserve successfully provisioned resources
**Your may need to try rollback and redeploy stack for CFDistribution because it asyncs CDN resources across aws network and takes long time up to half an hour.**

4. Customize your application source files.
| Key         | Value                                                                |
| :---        |:---                                                                  |
| APIEndpoint | https://b8loh8qf28.execute-api.ap-northeast-3.amazonaws.com/v1/hello |
| BucketName  | react-cors-spa-E3CVB3FLQBYYC2                                        |

5. 

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ROADMAP -->
## Roadmap

- [x] Fix **You have attempted to create more buckets than allowed** issue resulting in rollback and deployment failure during cloudformation stack deployment.(A tool to delete unused buckets)

See the [open issues](https://github.com/yuzukicat/cloudfront-s3-actions-react/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTRIBUTING -->
## Contributing

If you are familar with github actions, CI/CD or AWS, you are welcome to join and development automated deployment tools

1. Clone the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

Emails:

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

Yuzuki.Cat - dawei.jiang@nowhere.co.jp

Project Link: [https://github.com/yuzukicat/cloudfront-s3-actions-react](https://github.com/yuzukicat/cloudfront-s3-actions-react)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Please share useful links here for reference.

* [Deploy a React-based single-page application to Amazon S3 and CloudFront](https://docs.aws.amazon.com/prescriptive-guidance/latest/patterns/deploy-a-react-based-single-page-application-to-amazon-s3-and-cloudfront.html)
* [Code OSS Plugin | aws-cloudformation-yaml](https://marketplace.visualstudio.com/items?itemName=DanielThielking.aws-cloudformation-yaml)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://eyesjapan.atlassian.net/jira/software/projects/FOODAI/boards/231
[pull-request-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[pull-request-url]: https://git-codecommit.us-west-2.amazonaws.com/v1/repos/food-ai-app
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://eyesjapan.atlassian.net/jira/software/projects/FOODAI/boards/231
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[product-screenshot]: /src/assets/about/about-the-project.png




https://docs.aws.amazon.com/prescriptive-guidance/latest/patterns/deploy-a-react-based-single-page-application-to-amazon-s3-and-cloudfront.html

S3 URL: https://s3.ap-northeast-3.amazonaws.com/cf-templates-1xljco7p1ppqj-ap-northeast-3/2022243uMJ-react-cors-spa-stack.yaml

Stack failure options
Preserve successfully provisioned resources
