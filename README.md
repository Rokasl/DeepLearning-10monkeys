# 10 Monkey Species Image Dataset Analysis

Main code and the documentation is located in main.ipynb file. File typ is supported by Jupyter Notebook and should be viewed with it. 

Instruction to install Jupyter Notebook: http://jupyter.readthedocs.io/en/latest/install.html

## Retrained model

Graph location: './retrained_model/output_graph.pb'

This model can be tested either by running the script in main.ipynb file or by typing a command into the terminal. Example command:

```bash
python label_image.py \
--graph=./retrained_model/output_graph.pb --labels=./retrained_model/output_labels.txt \
--input_layer=Placeholder \
--output_layer=final_result \
--image=./input/validation/n8/n809.jpg
```

## Linear model

Graph location: '/linear_model/graph.pbtxt

This model can be tested by running the evaluation function in the main.ipynb file.