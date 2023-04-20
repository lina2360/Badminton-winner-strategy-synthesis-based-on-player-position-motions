# Badminton-winner-strategy-synthesis-based-on-player-position-motions

## The flows for the paper
1. download video from Youtube or other website, and use **preprocessing.ipynb** to do the screenshots for each 0.5 second from a video.

```
preprocessing.ipynb
```

   

2. input screenshots into the Mask-RCNN

```
mrcnn
```

3. predict diraction for each shuttlecock by Bi-LSTM and logic control

```
https://github.com/chi110356042/logic_badminton
```

4. automatic programs stage before SeqGAN 

hit,birdy,score,seqs.ipynb(HIT2SCORE)

seqgan_input.ipynb(SCORE2SEQ)

5. SeqGAN

execute-hiseqgan.py:(SEQGAN)

python execute-hiseqgan.py --data=wm5-normalize --filename=seqGAN_input_hs12_22.txt --target=id --generated_num=100 --total_batch=50 --batch_size=5 --seq_length=40

seqgan_output.ipynb(seqganoutput)

6. Statistic

final

