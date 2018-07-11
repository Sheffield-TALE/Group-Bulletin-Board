## Group-Bulletin-Board

[Get your Github student pack for unlimited private repositories](https://education.github.com/pack)

Please inform the onwers/research group members if the provided links are invalid.

### Table of contents:
- [Good paper for sharing](#Good-paper-for-sharing)
  - [Transfer learning](#Transfer-learning)
- [Computational resources](#Computational-resources)

### Good paper for sharing <a name="Good-paper-for-sharing"><a>

#### Transfer learning <a name="Transfer-learning"><a>
- [Learning transferable features with deep adaptation networks (DAN)](http://proceedings.mlr.press/v37/long15.pdf) [Long et al.,](http://ise.thss.tsinghua.edu.cn/~mlong/) in ICML, 2015. [[Code]](https://github.com/thuml/DAN)
- [Transfer Feature Learning with Joint Distribution Adaptation (JDA)](http://openaccess.thecvf.com/content_iccv_2013/papers/Long_Transfer_Feature_Learning_2013_ICCV_paper.pdf) [Long et al.,](http://ise.thss.tsinghua.edu.cn/~mlong/) in ICCV, 2013. [[Code]](http://ise.thss.tsinghua.edu.cn/~mlong/doc/joint-distribution-adaptation-iccv13.zip)
- [Domain adaptation via transfer component analysis (TCA)](http://www.aaai.org/ocs/index.php/IJCAI/IJCAI-09/paper/download/294/962) [Pan et al..,](http://www.ntu.edu.sg/home/sinnopan/index.html) in IJCA, 2009. 
- [Boosting for transfer learning (TrAdaBoost)](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.646.8484&rep=rep1&type=pdf) [Dai et al.,](https://scholar.google.co.uk/citations?user=AGR9pP0AAAAJ&hl=en) in ICML, 2007. 

#### Network Embedding 


#### Spectral Clustering for Higher-order Network Structures 



### Computational resources <a name="Computational-resources"><a>

  
- **_Sheffield HPC_**:

  - [Iceberg](http://docs.hpc.shef.ac.uk/en/latest/iceberg/index.html)

  - [ShARC](http://docs.hpc.shef.ac.uk/en/latest/sharc/index.html)

   Please contact Haiping for requesting access.

- **_Departmental Resources_**:

  - [Big memory nodes](http://docs.hpc.shef.ac.uk/en/latest/sharc/groupnodes/big_mem_nodes.html)

  - [Nvidia DGX-1](http://docs.hpc.shef.ac.uk/en/latest/sharc/groupnodes/dgx-1.html)

   Please contact Twin Karmakharm (t.karmakharm@sheffield.ac.uk) or RSE group (rse@shef.ac.uk) for requesting access.
   
- **_TALE Private Node on ShARC_**:  

  - Starting an interactive session

    Type `qrshx -P tale` to get access to the node (node156) with default 2GB real memory allocation. Use `top` to check how busy it is (currently idle, so please use it).
    
    If more memory e.g., 16GB is needed for your job, type `qrshx -P tale -q tale.q -l rmem=16G`. Be sure to request enough resource for your job in the interactive session, otherwise, the job will be killed without any warning or error message and you will be dropped out of the TALE node.

  - Submitting batch jobs

    Batch Jobs can be submitted to the TALE private node by adding the `-P tale -q tale.q` parameters, for example:

    ```
    #!/bin/bash
    #$ -P tale
    #$ -q tale.q

    echo "Hello world"
    ```
    More about the command for configuring batch jobs can be found on https://www.sheffield.ac.uk/cics/research/hpc/sharc/batch
   
- **_Data Storage_**:
  
  TALE group shared storage folder: "tale2". Only TALE group members have the access.
  
  Access research storage: https://www.sheffield.ac.uk/cics/research-storage/using-research-storage
  
  Access "tale2" from Sheffield HPC: Shared folders are not visible but accessible from Sheffield HPC (ShARC or iceberg) by using this command: `cd /shared/tale2/Shared`
