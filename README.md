# EduCEQ
****
A publicly available dataset and method for educational knowledge graph question answering

# 1 Note 
During the under review period, the dataset has been uploaded to figshare and can be viewed by editors and reviewers. It
will be fully released here as soon as the paper was accepted

# 2 dependencies
- pytorch>=1.2.0
- [transformers](https://github.com/huggingface/transformers)
- tqdm
- nltk
- shutil
  
# 3 Prepare Datasets
- [WebQSP](https://drive.google.com/drive/folders/1RlqGBMo45lTmWz9MUPTq-0KcjSd3ujxc?usp=sharing), which has been processed by [EmbedKGQA](https://github.com/malllabiisc/EmbedKGQA).
- [ComplexWebQuestions](https://drive.google.com/file/d/1ua7h88kJ6dECih6uumLeOIV9a3QNdP-g/view?usp=sharing), which has been processed by [NSM](https://github.com/RichardHGL/WSDM2021_NSM).
- [GloVe 300d pretrained vector](http://nlp.stanford.edu/data/glove.840B.300d.zip), which is used in the BiGRU model. After unzipping it, you need to convert the txt file to pickle file by 
``` shell
python pickle_glove.py --txt </path/to/840B.300d.txt> --pt </output/file/name>
```
# 4 Thanks
- TransferNet: https://github.com/shijx12/TransferNet
- EmbedKGQA: https://github.com/malllabiisc/EmbedKGQA
- NSM: https://github.com/RichardHGL/WSDM2021_NSM
