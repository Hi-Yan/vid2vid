

fork from https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix

a.sh is train cmd

python train.py --dataroot ./dataset/ucf-npy/ --dataset_mode v --model pix2pix --which_model_netG unet_256 --which_direction AtoB --norm batch --niter 10 --niter_decay 10 --batchSize 1 --name virtualkittidepth --depth 7 --max_dataset_size 150 --output_nc 3 --input_nc 3 --gpu_ids 0 --data_dir ./dataset/UCF/v_BabyCrawling**.avi --load_video 1  ：：run ok




Video2XYZ
已经实现：
<a href="https://mp.weixin.qq.com/s?__biz=MzA5MDMwMTIyNQ==&mid=2649292433&idx=1&sn=e3ca8c14e5e7454f8e9ac227ec9f4f63&chksm=8811e8d7bf6661c150d1bcb4204fccc34ad80086298b93821ad476aba9d85e6b44f5e066c80e&scene=21#wechat_redirect">[vid2dep demo show]  </a>
<a href="https://mp.weixin.qq.com/s?__biz=MzA5MDMwMTIyNQ==&mid=2649292657&idx=1&sn=080e7c029c952bbdd545bda2025ac0e8&chksm=8811e937bf666021543234e27fa9ddb9d37db4227bf0b47c319bb5a62d3af51be43d223d0334#rd">[vid2vid demo show]</a> 

<a href="https://v.qq.com/iframe/preview.html?vid=u1328ni8uvu&amp;width=500&amp;height=375&amp;auto=0" > [video generate demo: children]</a>

正在推进： vid2sped vid2angle vid2action vid2reward vid2nlp   ref: https://github.com/createamind/vid2vid/issues/3

更完善的期望是sensorfuse2representation,  representation2XYZ, SF2Rpstt2XYZ,

对于progressGAN--pix2pixHD想法是 can train pred angle /2(左右) /4(大左小左 大右小右) /8  图像的越来越精细到功能训练的准确度越来越高。

!Curiosity-driven Exploration by Self-supervised Prediction


new ref  https://github.com/createamind/keras-cpcgan
