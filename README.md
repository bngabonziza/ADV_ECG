# ADV_ECG
Code for Deep learning models for electrocardiograms are susceptible to adversarial attack

If you use the code in your research, please cite our paper:

Han, Xintian, et al. "Deep learning models for electrocardiograms are susceptible to adversarial attack." Nature medicine 26.3 (2020): 360-363.

The code is written in python 3.6 and pytorch 1.0.

The data is from https://physionet.org/challenge/2017/ It is read by python and saved in .npy file.

The signals file is too large. It cannot be uploaded to github. This is the Google drive link: https://drive.google.com/file/d/1u10ZvEilpZnOB4ls5ZAU5ywwf9g23oiB/view?usp=sharing 

Before you use the code, please download *raw_data.npy* from the link above and put it into the *data* folder.

In this folder:
  + *train.py*: Train the model and will save *best_model.pth* in *saved_model* folder. This training may take two days. One pretrained model is already saved in the *saved_model* folder.
  + *create_adv_pgd.py*: Generate adversarial examples by traditional attack method PGD.
  + *create_adv_conv_train.py*: Generate adversarial examples by smoothed attack method SAP.
  + *adv_measure_norm_all.py*: Generate new adversarial examples by adding Gaussian noise.
  + *check_concat.py*: Check that the concatenations of the new adversarial examples generated by *adv_measure_norm_all.py* are still adversarial examples.
  + *check_uniform.py*: Check that uniform samples from the band generated by *adv_measure_norm_all.py* are still adversarial examples.



