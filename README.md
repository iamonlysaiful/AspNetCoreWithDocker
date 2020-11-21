# Exploring ASP.NET Core With Docker hub for Windows & Linux

> I show here two way of creating docker image/container with/without docker compose file & I tried to show the whole process with screenshots and following step.
## New Repository on Docker Hub
  1. **Sign In** on docker.com
  2. After sign in select **Repositories** from dashboard Menu

![Image 0](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/0.png?raw=true)

  3. From Repositories Page Click **Create Repository**
  5. Fill up Form, Select Public/Private whatever you want and Click **Create**

![Image 1](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/1.png?raw=true)

  6. Named Repository Created
  
![Image 2](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/2.png?raw=true)

## Hosting Docker Image of ASP.NET Core App
  1. Create or Open .NET Core App
  2. Here my App running on **61756** port

![Image 3](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/3.png?raw=true)
  
  3. Right **Click on project** & **Click Add** then **Click Docker Support**
  4. Then Select **Target OS**, In my case Linux

![Image 4](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/4.png?raw=true)

  5. Docker File added in your project with auto generated Config
  6. Docker Image Created on Default container

![Image 5](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/5.png?raw=true)

  7. **Edit Docker File** configuration according your project location

![Image 6](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/6.png?raw=true)
  
  8. Open **Project Location** on Command Prompt or PowerShell
  9. Run **build** command

![Image 7](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/7.png?raw=true)

  10. Successfully built

![Image 8](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/8.png?raw=true)

  11. Here is my Newly Built Image on local Docker hub
  12. Run Image on your machine from hub with desired Port 

![Image 9](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/9.png?raw=true)

  13. Here my Image running on Hosted Port

![Image 10](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/10.png?raw=true)

  14. Here I enlisted the command of stop container

![Image 11](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/11.png?raw=true)

## Hosting Docker Image of ASP.NET Core App Using Compose
  1. After Creating or Opening App
  2. By right clicking on Project Click Add & then Click Container Orchestrator Support
  3. Select Container & Target OS type

![Image 12](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/12.png?raw=true)
![Image 13](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/13.png?raw=true)
![Image 14](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/14.png?raw=true)

  4. Docker File & docker-compose added on project
  5. Image Created on Default Container

![Image 15](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/15.png?raw=true)

  6. By Opening docker-compose.yml rename Image name as your docker hub Repository name

![Image 16](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/16.png?raw=true)
![Image 17](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/17.png?raw=true)

  7. Set docker-compose Build mode  Release
  8. Build or Rebuild docker-compose

![Image 18](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/18.png?raw=true)

  9. Here is  Newly built image

![Image 19](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/19.png?raw=true)

  10. Run Image on your machine from hub with desired Port
  11. Here my application is running on Hosted Port  

![Image 20](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/20.png?raw=true)
![Image 21](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/21.png?raw=true)

## Pushing Docker Image to Docker Hub
  1. Run docker push command with Repository name

![Image 22](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/22.png?raw=true)

  2. Here you can see New Pushed Image with latest tag

![Image 23](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/23.png?raw=true)

## Pulling Docker Image from Hub on Linux
  1. Browse docker Repositories and copy Pull command

![Image 24](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/24.png?raw=true)

  2. Login to docker
  3. Pull hosted repositories from windows by  copied Pull command
  4. Here is my Pulled Image

![Image 25](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/25.png?raw=true)
## Running Pulled Image on Linux
  1. Run Image on your Linux machine from hub with desired Port

![Image 26](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/26.png?raw=true)

  2. Here my application is running on Hosted Port  in my Linux machine

![Image 27](https://github.com/iamonlysaiful/AspNetCoreWithDocker/blob/main/DemoBackendAPIForDocker/Screenshots/27.png?raw=true)
