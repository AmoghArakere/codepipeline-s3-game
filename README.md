# Continuous Deployment using AWS Code Pipeline and S3
![Screenshot 2024-05-17 015032](https://github.com/AmoghArakere/codepipeline-s3-game/assets/90240269/9c7336aa-cfe8-4445-85fe-ef95b5e03542)
![Screenshot 2024-05-17 014648](https://github.com/AmoghArakere/codepipeline-s3-game/assets/90240269/0de3385a-4082-4b79-af09-82fd7bf6ae48)



## TL;DR
Code for a game is hosted in GitHub.  We create an S3 bucket for static website hosting, then create a continuous deployment pipeline (using AWS Code Pipeline) to automatically deploy the code whenever changes are made.

## The Game
A simple memory matching game.  The user clicks two cards (images of memes) to try to match them.  If there's a match, the cards disappear from the board.  If there's no match, the cards are flipped back to their blank side so the user can try again.

## The Deployment Environment
The code will be deployed and hosted in S3.

## The Deployment Pipeline
The pipeline is created using AWS Code Pipeline.  The pipeline pulls the code from GitHub, and deploys it to S3 whenever a change is detected in the code.
