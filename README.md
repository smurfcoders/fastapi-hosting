# Fastapi-hosting
Complete Guide for hosting fastapi. Below are the steps for hosting fastapi on aws ec2 and access it through anywhere on the internet.


<h1 align="center">
  <a href="https://github.com/smurfcoders/fastapi-hosting">
    <img src="https://raw.githubusercontent.com/smurfcoders/fastapi-hosting/master/Smurf%20coders.jpg">
  </a>
</h1>

<div align="center">
  Host any Fastapi application by using this tutorial - Subscribe to our youtube channel !
</div>

<div align="center">
<br />

[![license](https://img.shields.io/github/license/dec0dOS/amazing-github-template.svg?style=flat-square)](LICENSE)

[![PRs welcome](https://img.shields.io/youtube/channel/views/UCmkU-qYoP19uM3ueLyhxEMg?color=red)](https://www.youtube.com/channel/UCmkU-qYoP19uM3ueLyhxEMg)
[![made with hearth by smurfcoders](https://img.shields.io/badge/made%20with%20%E2%99%A5%20by-smurfcoders-ff1414.svg?style=flat-square)](https://github.com/smurfcoders)

</div>


### Built With

- [Fastapi](https://github.com/tiangolo/fastapi)
- [Python](https://www.python.org/)
- [AWS](https://aws.amazon.com/)

## Getting Started

### Prerequisites

We assume that you have a amazon ec2 instance.
In this [tutorial](https://www.youtube.com/channel/UCmkU-qYoP19uM3ueLyhxEMg) we have used ubuntu with [aws free tier](https://aws.amazon.com/free/) and instance type is t2.micro(1 gb ram).

After you enter the instance by ssh or any other method update the instance first by using below command:

```sh
sudo apt-get update
```

Command to install python :

```sh
sudo apt install python3-pip
```


Command to install git to clone this repository :

```sh
sudo apt install git
```

Command to install git to clone this repository you can use your repository git url which you want to host :

```sh
sudo git clone https://github.com/smurfcoders/fastapi-hosting.git
```

Command to change location into the cloned folder you can use your repository name :

```sh
cd fastapi-hosting
```

Command to install all the requirements required for the project to run in our case we have created requirements.txt file you can also create your own requirements :

```sh
pip install -r requirements.txt
```

Command to run the API :

```sh
python3 -m uvicorn main:app --host 0.0.0.0 --port 8000
```

After running go to AWS instance --> Security tab --> Edit inbound rules --> create rule --> Enable access from anywhere.<br>
Go to the public ip provided by the instance add :8000 in the end as our api is running at that particular port.

That's it you can now access your Fastapi from anywhere.

> Got any doubts feel free to ask : [GitHub Discussions](https://github.com/smurfcoders/fastapi-hosting/discussions).


## License

This project is licensed under the **MIT license**. Feel free to edit and distribute this template as you like.

See [LICENSE](LICENSE) for more information.

## Acknowledgements

Thanks for reading do let us know any interesting topics to teach on our [youtube channel!](https://www.youtube.com/channel/UCmkU-qYoP19uM3ueLyhxEMg)

