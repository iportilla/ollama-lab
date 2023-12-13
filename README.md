# Ollama Lab

## Ollama notebooks Demo


<h1 align="center" style="border-bottom: none;">🔎 Ollama 101 </h1>
<h3 align="center">Ollama: Get up and running with large language models, locally.
Run Llama 2, Code Llama, and other models. Customize and create your own.</h3>


### Flow

In this topic, you'll follow a series of hands-on exercises that demonstrate how to use Ollama. You'll start with the basics: creating and running your Ollama environment. By the end of the course, you'll get a brief introduction to running LLMs locally.



Enjoy this topic!

<h3>APPM-5720</h3>

Install Ollama if you have enough RAM & Storage  (8 GB RAM, 10 GB Disk) from:

[https://ollama.ai/](https://ollama.ai/)

Else use CURC or AWS VM with

```
docker run -d -v ollama:/root/.ollama -p 11434:11434 --name ollama ollama/ollama

docker exec -it ollama ollama run orca-mini
```

### CURC

```
singularity pull ollama.sif docker://ollama/ollama:latest

singularity run ollama.sif

singularity exec ollama.sif ollama run orca-mini
```

Watch for `~/home/` size with `du -H .` or `curc-quota`
https://ollama.ai/blog/ollama-is-now-available-as-an-official-docker-image

See this page for details

https://github.com/jmorganca/ollama


See examples in Python [Folder](python)

Also see:

Jetson Nano
https://github.com/jmorganca/ollama/blob/main/docs/tutorials/nvidia-jetson.md


Ollama Notebook
https://github.com/jmorganca/ollama/tree/main/examples/jupyter-notebook


Ollama Kubernetes
https://github.com/jmorganca/ollama/tree/main/examples/kubernetes
