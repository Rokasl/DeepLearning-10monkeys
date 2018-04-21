# 10 Monkey Species Image Dataset Analysis

Main code and the documentation is located in main.ipynb file. File type is supported by the Jupyter Notebook and should be viewed and used with it. 

Instruction to install Jupyter Notebook: http://jupyter.readthedocs.io/en/latest/install.html

The documentation without any code is located in report.pdf file.

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

Due to graph's size (around 800MB) it was not possible to upload it here, however it can easily be newly generated just by running the script in main.ipynb file (takes around 2 minutes). The other option is to just look through cached output in the main.ipynb file.

After training, graph location is: '/linear_model/graph.pbtxt

This model can be tested by running the evaluation or prediction blocks in the main.ipynb file.
