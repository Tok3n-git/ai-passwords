# ai-passwords

This is a collection of password lists in which I have trained various deep learning algorithms to try to come up with passwords. A full report of results exists in each directory.

## Tests Run

* **gpt2-small**: Using minimaxir's [gpt-2-simple](https://github.com/minimaxir/gpt-2-simple) with GPT2-small and some of the [hashes.org](https://hashes.org) "founds" dataset. 

## Performance

This table lists approximate performance metrics for these models. 

Metrics are:

* **Model Name**: The model/folder used to generate the password list.
* **Generated**: The amount of passwords generated by the model.
* **Unique**: The amount of unique passworss generated by the model.
* **In Training Set**: The amount of generated passwords that exist in the training dataset.
* **PW/sec**: Approximate password generation per second, raw.
* **Cracks/sec.**: Approximate novel passwords yielding cracks of the validation dataset per second.
* **Rig**: The computer specifications used against the model. Often I borrow old/recycled hardware from friends to run my GPUs.

| Model Name | Generated | Unique    | In Training Set | PW/sec. | Cracks/Sec. | Rig |
|------------|-----------|-----------|-----------------|---------|-------------|-----|
|gpt2-small  | 4,726,912 | 4,053,784 | 822,690         | 111     | 12.17       | A   |


### Rig Specifications

This contains hardware specifications used to run the model.

#### Rig A "thehaswell"

* Intel Core i7-4790K (Devil's Canyon)
* 32GB DDR3 RAM
* 1 TB NVMe SSD (Samsung 960 Evo)
* AMD Radeon VII (VBIOS version: 113-D3600200-106)
* Ubuntu 18.04.3 LTS, ROCm 2.9.6

# License

MIT License
