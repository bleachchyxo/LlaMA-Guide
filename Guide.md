# Installing LlaMA 


## Setting llama.cpp

Here are the steps for the LLaMA-7B model.

    git clone https://github.com/ggerganov/llama.cpp

Once the code been downloaded

    cd llama.cpp
    make

And to ensure we use just the CPU cores

    make LLAMA_OPENBLAS=1

## Downloading a model

https://huggingface.co/TheBloke/WizardLM-7B-uncensored-GGML/tree/main

Here is the binarie that goes into `/models`, once inserted there you can run your local model with the next command:

     make -i  && ./main -m ./models/WizardLM-7B-uncensored.ggml.q5_1.bin -p "what is the difference between NVMe and SATA?" -n 512
     ./main -ins -m ./models/WizardLM-7B-uncensored.ggmlv3.q8_0.bin -n 512
    
