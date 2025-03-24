Entoa-TTS is a dataset composed of 20 audio files and transcriptions (both manual and automatic by WhisperX), from NURC-SP Minimal Corpus: 6 Formal Elocutions (EF) totaling 4h28min52s; 5 formal dialogues between the speakers, with the presence of a documenter (D2) totaling 5h22min07s; 9 interviews about different topics, carried out by an interviewer with the interviewee (DID) totaling 6h11min20s. Although NURC-SP Minimal Corpus has 21 pairs of audio-transcription, one of them (SP_D2_062) was removed as its audio quality was not good for training TTS.

To compose the dataset part called "prosodic" it was used only terminal intonational units (terminal boundaries mark the conclusion of the utterance) from NURC-SP Minimal Corpus. For the part called "automatic" the 20 audio files of NURC-SP Minimal Corpus were segmented and transcripted by WhisperX. This dataset is used to compare the training of TTS models with terminal intonational units and with the segments generated by WhisperX.  The prosodic parte of Entoa-TTS has ___todo___ hours and the automatic part has ___todo___ hours.

# Dataset
[Hugging Face Dataset](https://huggingface.co/datasets/nilc-nlp/NURC-SP_ENTOA_TTS)

# Models
- **FastSpeech2**: [FastSpeech2 info](https://github.com/nilc-nlp/entoa-tts/tree/main/models/FastSpeech2)


# Examples - FastSpeech2 

<table>
  <tr>
    <th>ID</th>
    <th>Speech</th>
    <th>Ground Truth</th>
    <th>FastSpeech2 CMLTTS</th>
    <th>FastSpeech2 CMLTTS + ENTOA-PROSODIC</th>
    <th>FastSpeech2 CMLTTS + ENTOA-AUTOMATIC</th>
  </tr>
  
<tr>  
  <td>01</td> 
  <td>eu quase não vou ao cinema teatro...</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_7.36_9.50.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/eu quase não vou ao cinema teatro....wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/eu quase não vou ao cinema teatro....wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/eu quase não vou ao cinema teatro....wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>02</td>
  <td>ah às vezes eu vou... </td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_9.50_10.79.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/ah às vezes eu vou... .wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/ah às vezes eu vou....wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/ah às vezes eu vou....wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>03</td>
  <td>eu tenho ido a teatro.</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_20.58_21.49.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/eu tenho ido a teatro..wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/eu tenho ido a teatro..wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/eu tenho ido a teatro..wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>04</td>
  <td>deve ser como na televisão</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_487.27_488.30.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/deve ser como na televisão.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/deve ser como na televisão.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/deve ser como na televisão.wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>05</td>
  <td>então no teatro eu acho que é bem mais difícil...</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_567.37_570.67.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/então no teatro eu acho que é bem mais difícil....wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/então no teatro eu acho que é bem mais difícil....wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/então no teatro eu acho que é bem mais difícil....wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>06</td>
  <td>a televisão é horroroso quando eles estão fazendo programa.</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_572.43_574.93.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/a televisão é horroroso quando eles estão fazendo programa..wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/a televisão é horroroso quando eles estão fazendo programa..wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/a televisão é horroroso quando eles estão fazendo programa..wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>07</td>
  <td>eu sei que não há preparação toda.</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_749.16_751.35.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/eu sei que não há preparação toda..wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/eu sei que não há preparação toda..wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/eu sei que não há preparação toda..wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>08</td>
  <td>porque o grupo que trabalha em hair é enorme né</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_791.94_793.72.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/porque o grupo que trabalha em hair é enorme né.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/porque o grupo que trabalha em hair é enorme né.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/porque o grupo que trabalha em hair é enorme né.wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>09</td>
  <td>tenho impressão que ali levou tanto tempo de ensaio</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_798.97_800.89.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/tenho impressão que ali levou tanto tempo de ensaio.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/tenho impressão que ali levou tanto tempo de ensaio.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/tenho impressão que ali levou tanto tempo de ensaio.wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>10</td>
  <td>me chocou tremendamente</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_838.92_840.07.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/me chocou tremendamente.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/me chocou tremendamente.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/me chocou tremendamente.wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>11</td>
  <td>eu saber que o filme é bom</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_997.24_998.36.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/eu saber que o filme é bom.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/eu saber que o filme é bom.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/eu saber que o filme é bom.wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>12</td>
  <td>eu gostei bastante</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_1086.45_1087.34.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/eu gostei bastante.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/eu gostei bastante.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/eu gostei bastante.wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>13</td>
  <td>eu me lembro de vários filmes não lembro os nomes</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_1176.36_1178.28.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/eu me lembro de vários filmes não lembro os nomes.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/eu me lembro de vários filmes não lembro os nomes.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/eu me lembro de vários filmes não lembro os nomes.wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>14</td>
  <td>por isso é que eu deixo de ir ao cinema</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_1187.18_1188.64.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/por isso é que eu deixo de ir ao cinema.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/por isso é que eu deixo de ir ao cinema.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/por isso é que eu deixo de ir ao cinema.wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>15</td>
  <td>hoje tá tudo meio louco né</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_1203.43_1204.54.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/hoje tá tudo meio louco né.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/hoje tá tudo meio louco né.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/hoje tá tudo meio louco né.wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>16</td>
  <td>assisti em araraquara.</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_1218.75_1219.65.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/assisti em araraquara..wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/assisti em araraquara..wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/assisti em araraquara..wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>17</td>
  <td>eu num lembro o nome do filme...</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_1238.92_1240.34.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/eu num lembro o nome do filme....wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/eu num lembro o nome do filme....wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/eu num lembro o nome do filme....wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>18</td>
  <td>a molecada adorou.</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_1221.63_1222.49.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/a molecada adorou..wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/a molecada adorou..wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/a molecada adorou..wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>19</td>
  <td>eles adoraram o filme...</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_1223.27_1224.60.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/eles adoraram o filme....wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/eles adoraram o filme....wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/eles adoraram o filme....wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>20</td>
  <td>porque eu saio cansada mesmo</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_1268.89_1270.11.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/porque eu saio cansada mesmo.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/porque eu saio cansada mesmo.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/porque eu saio cansada mesmo.wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>21</td>
  <td>eu fico numa tensão nervosa</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_1270.11_1271.29.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/eu fico numa tensão nervosa.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/eu fico numa tensão nervosa.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/eu fico numa tensão nervosa.wav'}}" type="audio/mpeg"></audio></td> 
  
</tr>

<tr>  
  <td>22</td>
  <td>nós saímos pra ir ao teatro.</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_1294.60_1295.66.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/nós saímos pra ir ao teatro..wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/nós saímos pra ir ao teatro..wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/nós saímos pra ir ao teatro..wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>23</td>
  <td>não conseguimos entrar fomos assistir esse filme.</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_1296.22_1297.96.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/não conseguimos entrar fomos assistir esse filme..wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/não conseguimos entrar fomos assistir esse filme..wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/não conseguimos entrar fomos assistir esse filme..wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>24</td>
  <td>eu acho que influi bastante</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_1325.38_1326.62.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/eu acho que influi bastante.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/eu acho que influi bastante.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/eu acho que influi bastante.wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>25</td> 
  <td>eu acho que teatro tá bem mais caro</td>
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_1560.80_1562.37.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/eu acho que teatro tá bem mais caro.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/eu acho que teatro tá bem mais caro.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/eu acho que teatro tá bem mais caro.wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>26</td>  
  <td>eu acho que o público pre prefere cinema ainda</td-->  
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_1574.34_1576.29.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/eu acho que o público pre prefere cinema ainda.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/eu acho que o público pre prefere cinema ainda.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/eu acho que o público pre prefere cinema ainda.wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>27</td> 
  <td>eu não entendi a pergunta</td-->  
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_1786.32_1787.49.wav'}}" type="audio/mpeg"></audio></td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/eu não entendi a pergunta.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/eu não entendi a pergunta.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/eu não entendi a pergunta.wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>28</td>  
  <td>eu acho que o cinema tá perdendo viu</td> 
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_1935.41_1937.01.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/eu acho que o cinema tá perdendo viu.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/eu acho que o cinema tá perdendo viu.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/eu acho que o cinema tá perdendo viu.wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>29</td> 
  <td>o que eu noto é isso</td-->  
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_2007.04_2007.78.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/o que eu noto é isso.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/o que eu noto é isso.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/o que eu noto é isso.wav'}}" type="audio/mpeg"></audio></td>   
</tr>

<tr>  
  <td>30</td> 
  <td>principalmente nos fins de semana</td-->  
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/ground_truth/SP_DID_234_seg_2121.79_2123.22.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts/speaker_25/principalmente nos fins de semana.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_pros/speaker_12249/principalmente nos fins de semana.wav'}}" type="audio/mpeg"></audio></td>   
  <td><audio controls preload style="width: 150px; height:40px;"><source src="{{ 'experiments/FastSpeech2/output/cmltts_entoa_auto/speaker_12249/principalmente nos fins de semana.wav'}}" type="audio/mpeg"></audio></td>   
</tr>

 
</table>
