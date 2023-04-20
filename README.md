# Badminton-winner-strategy-synthesis-based-on-player-position-motions

## The flows for the paper
1. download video from Youtube or other website, and use

preprocessing.ipynb

to do the screenshots for each 0.5 second from a video.
2. input screenshots into the Mask-RCNN

mrcnn

d:

https://github.com/chi110356042/logic_badminton

hit,birdy,score,seqs.ipynb(HIT2SCORE)

seqgan_input.ipynb(SCORE2SEQ)

execute-hiseqgan.py:(SEQGAN)

python execute-hiseqgan.py --data=wm5-normalize --filename=seqGAN_input_hs12_22.txt --target=id --generated_num=100 --total_batch=50 --batch_size=5 --seq_length=40

seqgan_output.ipynb(seqganoutput)

final

