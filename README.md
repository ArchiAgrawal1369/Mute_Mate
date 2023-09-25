# Mute_Mate

Mute Mate is a lip-reading system that has been specifically designed to aid mute individuals during online conferences. With the rising popularity of remote communication, the need to address communication challenges faced by those who cannot vocalize their thoughts becomes crucial. Mute Mate utilizes advances computer vision and machine learning techniques to accurately interpret lip movements, enabling efficient communication. 

## Project Structure
<ul>
  <li>
    `models/` stores the model checkpoint.
  </li>
  <li>
    `app/utils.py` contains data loading functions with preprocessing steps.
  </li>
  <li>
    `app/modelutil.py` describes the model architecture.
  </li>
  <li>
    `app/streamlitapp.py` defines the structure of Streamlit application.
  </li>
  <li>
    `app/test_video.mp4` and `app/animation.gif` will be replaced by current prediction video.
  </li>
</ul>

## Development Steps
<ol>
<li>The subset of the GRID Corpus dataset used for this project can be downloaded from <a href="https://drive.google.com/uc?id=1YlvpDLix3S-U8fd-gqRwPcWXAXm8JwjL">here</a>.</li>
<li>Data preprocessing is performed on the videos as well as their corresponding alignments.</li>
<li>
  STCNN + BiLstm model architecture is defined with softmax activation. 
</li>
<li>
  Model is trained and tested on the two sets of data.
</li>
  <li>
    Finally, it has been integrated into a streamlit based application to make predictions. `streamlit run streamlitapp.py` will be used to run the application.
  </li>
</ol>

## Further Reading
Read more about lip-reading model at https://arxiv.org/abs/1611.01599
