# Evil Corp. release repo
## prerequisites:
 - Docker
 - gh token
## installation steps:
1. Create new release (optional)
2. Head to releases page
3. After a while there should be docker-compose.yml file there with latest revisions of both backend and frontend images
4. Download it to machine of your choosing
5. Login to docker ghcr.io repo using:
    ```
    echo ${ your_token } | docker login ghcr.io -u ${ your_username } --password-stdin
    ```
    *remember that your token needs to have correct permissions*
6. Start docker containers:
    ```
    docker-compose up -d
    ```

## Known limitations:
- no staging for packages
- no docker-compose for qa branches

:(
