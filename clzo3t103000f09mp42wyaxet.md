---
title: "Playlists on Autopilot: Manage Spotify with Terraform"
seoTitle: "Automate Spotify Playlists with Terraform"
datePublished: Sat Aug 10 2024 12:20:09 GMT+0000 (Coordinated Universal Time)
cuid: clzo3t103000f09mp42wyaxet
slug: playlists-on-autopilot-manage-spotify-with-terraform
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1723286473196/a6e157d8-7040-490c-9fbc-87d357f9a77a.png
tags: projects, devops, terraform, iac, devops-articles, devops-journey

---

### Project Overview

This project showcases how to harness the power of Terraform to create and manage multiple Spotify playlists effortlessly. With Terraform's automation capabilities, you can streamline your playlist organization and tailor your music experience effortlessly. Say goodbye to manual playlist management and let Terraform handle it all for you—transforming how you curate and enjoy your favorite tunes!

### Starting Essentials

1. **"Terraform Ready?"**: Get Terraform set up on your system to start building!
    
2. **"Docker on Deck?"**: Ensure Docker is installed and running smoothly.
    
3. **"Spotify Account in Hand?"**: Have a Spotify account ready (premium not required)!
    
4. **"Spotify Dev Setup"**: Sign up for a Spotify Developer account and snag your Client ID and Secret.
    
5. **"Spotify Terraform Plugin"**: Install and configure the Spotify provider to connect with Terraform.
    
6. **"VS Code Vibes"**: Use VS Code for an effortless editing experience with Terraform files.
    

### How to Rock This Project

### 1\. **Kickoff Your Terraform Code**

Get your Terraform project up and running.

1. **Set Up Shop**: Create a new directory for your Terraform project and dive in via your terminal.
    
2. **Start Coding**: Create a file named [`main.tf`](http://main.tf) to begin your configuration.
    

#Bonus: Run `terraform -v` to confirm Terraform is installed and ready to go!

### 2\. **Plug into Spotify**

In [`main.tf`](http://main.tf), set up the Spotify provider:

```plaintext
provider "spotify" {
  api_key = "?"
}
```

### 3\. Grab Your API Key

To connect with Spotify’s API, you'll need a Client ID and Client Secret.

### 4\. Kickstart your App

1. Navigate to [Spotify Developer Dashboard.](https://developer.spotify.com/)
    
2. **Log In**: Use your Spotify account credentials.
    
3. **Create Your App**: Click on “Create an App” to get started!
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1723289090706/2a1358b4-0530-42a8-8bbe-1039619f43e3.png align="center")
    
4. **Complete the Form & Launch Your App**: Fill in the details and hit "Create App" to bring your project to life!
    

| Name | Description |
| --- | --- |
| My Playlist through Terraform | Create multiple Spotify playlists using Terraform. |

5. **Set Your Redirect URI**: Use [`http://localhost:27228/spotify_callback`](http://localhost:27228/spotify_callback) as the callback URL.
    

Hit **Settings** and jot down your Client ID and Client Secret—these are your keys to the Spotify kingdom!

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1723289575243/a7e528a2-a2ba-4755-8d0f-4c4bb529100c.png align="center")

### 5\. Store Your Credentials

Create a `.env` file to securely stash your Spotify Client ID and Secret!

```plaintext
SPOTIFY_CLIENT_ID=<your_spotify_client_id>
SPOTIFY_CLIENT_SECRET=<your_spotify_client_secret>
```

### 6\. Fire Up the Spotify Auth App and Grab Your API Key

Ensure Docker Desktop is up and running, then launch the authorization proxy server to get your API key!

```plaintext
docker run --rm -it -p 27228:27228 --env-file .env ghcr.io/conradludgate/spotify-auth-proxy
```

I have my .env file in the same project folder, that's why I am using `.env`

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1723290155399/d2ebd1fc-263a-490b-b82e-bab5241b5592.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1723290247745/2af090e4-ad9f-41c8-882c-f9192164ed45.png align="center")

You should see the “Authorization Successful” message—your access is now locked and loaded!

### 7\. Kick Off and Apply Your Terraform Configuration

1. **Initialize**: Fire up your Terraform setup by running the initialization command.
    

```plaintext
terraform init
```

2. **Apply**: Execute your Terraform configuration to bring your setup to life!
    

```plaintext
terraform apply
```

### 8\. Check Out Your Playlists on Spotify

Once Terraform has done its magic, log in to your Spotify account and see your new playlists—complete with all the tracks you specified!

*Here are some snapshots of my playlist in action:*

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1723290643337/a340f53d-7e0a-4873-bc48-0cb7b55575f9.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1723290672476/2bcb77b2-a026-4932-9da0-87b3244ca547.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1723290708648/8f9957b9-4aac-4144-b2ad-176f696d8573.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1723291518954/040fcf4b-f2b8-4601-94dc-55370d2b9123.png align="center")

## **Wrap-Up**

With these steps, you've just turned playlist management into a breeze! Automate your Spotify playlist creation with Terraform to save time and keep everything consistently awesome. Feel free to tweak and tailor your playlists for any occasion and let your music flow effortlessly!

Here’s where you can check out the project on GitHub: [GitHub Link](https://github.com/Callmeanurag/Terraform_Spotify_Project) 😉

---

Hey there! I’m Anurag Raj, a DevOps wizard with 3 years of expertise in supercharging operations and driving seamless CI/CD magic.

Ready to connect? Just click the link and say "[Hello](https://www.linkedin.com/in/anurag-raj-8975b0128/)"!