# my-first-solana-project-series-II-part-11

### This project is part of a series and includes a video.

See [Here](https://github.com/elicorrales/blockchain-tutorials/blob/main/README.md) for the overall document that
refers to all the series.  
  
## In this video we learn how to  
- display any data that is passed in from the client to the on-chain program
- control which program id (keypair) we wish to use when deploying an on-chain program
- deploy and run multiple versions of the program by which program id we use to invoke it


Useful commands:
```
solana config get
```
The above line shows you what your local config has.  Two important values would be the URL (for this series -we are using ```localhost```) and the ```Keypair Path```.
  
<br/>

```
solana-test-validator  # keep this running in a terminal
```
I mostly run the above local validator in the current project directory.  It creates a directory ```test-validator```.  Make sure that your local config ```solana config get``` is pointing to the correct ```wallet```.  
I mostly run the local validator with the ```--reset``` flag - starts fresh every time. Means you'll have to re-deploy  your on-chain program AND you'll lose any accounts your client created.  
<br/>
```
solana logs # keep this running in another terminal
```
The above will display any output related to your on-chain deployed program, or certain command-line solana commands, such as ```deploy```.  
<br/>
```
solana program show --programs
```
The above line will let you know if your program(s) are currently deployed.  
<br/>
