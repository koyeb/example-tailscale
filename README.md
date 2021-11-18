<div align="center">
  <a href="https://koyeb.com">
    <img src="https://www.koyeb.com/static/images/icons/koyeb.svg" alt="Logo" width="80" height="80">
  </a>
  <h3 align="center">Koyeb Serverless Platform</h3>
  <p align="center">
    Tailscale on Koyeb
    <br />
    <a href="https://koyeb.com">Learn more about Koyeb</a>
    ·
    <a href="https://koyeb.com/docs">Explore the documentation</a>
    ·
    <a href="https://koyeb.com/tutorials">Discover our tutorials</a>
  </p>
</div>


## About Koyeb and Tailscale

Koyeb is a developer-friendly serverless platform to deploy apps globally. No-ops, servers, or infrastructure management.

Tailscale is a VPN service that makes the devices and applications you own accessible anywhere in the world, securely and effortlessly.
It enables encrypted point-to-point connections using the open source WireGuard protocol, which means only devices on your private network can communicate with each other.

This repository showcases how to deploy an application on Koyeb and makes it only accessible via your Tailscale private network. This is useful when you need to deploy an internal app without exposing it to the internet.

## Getting Started

This example deploy a Golang Gin application on Koyeb and makes it only accessible via your Tailscale private network.

### Requirements

You need a Koyeb account and a [Tailscale account](https://tailscale.com/login) to successfully deploy and run this application. If you don't already have an account, you can sign-up for free [here](https://app.koyeb.com/auth/signup).

### Deploy using the Koyeb button

#### A Golang Gin application you can reach via your Tailscale private network.

The fastest way to deploy the Golang Gin application using Tailscale on Koyeb is to click the **Deploy to Koyeb** button below.

[![Deploy to Koyeb](https://www.koyeb.com/static/images/deploy/button.svg)](https://app.koyeb.com/deploy?type=docker&image=koyeb/tailscale-on-koyeb&ports=8080;http&name=tailscale-on-koyeb&env[TAILSCALE_AUTHKEY]=&env[TAILSCALE_HOSTNAME]=koyeb)

Clicking on this button brings you to the Koyeb App creation page with everything pre-set to launch this application.

Once deployed, you can access the application using:

```
curl http://TAILSCALE_DEVICE_IP:8080
```

_To modify this application example, you will need to fork this repository. Check out the [fork and deploy](#fork-and-deploy-to-koyeb) instructions._

## Contributing

If you have any questions, ideas, or suggestions regarding this application sample, feel free to open an [issue](//github.com/koyeb/example-tailscale/issues) or fork this repository and open a [pull request](//github.com/koyeb/example-tailscale/pulls).

## Contact

[Koyeb](https://www.koyeb.com) - [@gokoyeb](https://twitter.com/gokoyeb) - [Slack](http://slack.koyeb.com/)
