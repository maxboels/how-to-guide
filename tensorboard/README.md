

## 1. open new command line window connect to the server

### Type "hostname" in terminal to get your "HOSTNAME":
    ```
    ssh -N -f -L <LOCALPORT>:<HOSTNAME>:<DGXPORT> mboels@h1
    ```

    ```
	ssh -N -f -L 11093:localhost:11093 aicheadnode
    ```

## 2. Activate conda env with tensorboard and tensorflow installed:
    ```
    conda activate tensorboard
    ```

## 3. Run this command in your remote-server: 
    ```
    tensorboard --logdir=/your/path/to/logs --port=11093
    ```
