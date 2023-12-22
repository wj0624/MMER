# 한양대학교 정보융합전공 졸업 논문_4조
👨🏻‍🤝‍👨참여자 : 김희*, 백성*, 백신*, 안소*, 임원*, 임하*


## 주제 : 한국인 감정 인식을 위한 멀티모달모델 제안 및 OTT 콘텐츠를 통한 검증
(Proposal for a Multi-Modal AI model for Korean Emotion Recognition And Validation through OTT Contents)


### 1. __감정 분류__ 
 😊행복, 😢슬픔, 😮놀람, 😠분노, 😱공포, 😩혐오, 😶중립
### 2. __학습 데이터__
 1. 🔊💬음성-텍스트 모델 : ETRI 'KEMDy19'
 2. 👨‍🦲표정 모델 : AI hub '한국인 감정인식을 위한 복합영상 데이터’ + FER-2013
 3. 🗣최종 모델 : AI hub '감정 분류용 데이터셋'
### 3. __모델 설명__
  *  RoBERTa 기반의 텍스트 모델, Wav2Vec 2.0 기반의 음성 모델, Efficient Net 기반의 표정 모델
  *  Multihead-Attention으로 통합된 음성-텍스트 모델과 표정 모델에서 추출한 신뢰도 점수를 활용하여 최종 모델(LGBM) 학습
  *  최종 모델 결합 구조

     ![image](https://github.com/wj0624/MMER/assets/128574107/8eea4c36-eb1c-42c7-8b3e-7a81a0685883)

### 4. __결과__
*  최종모델 LGBM 학습결과 : __accuracy 0.81__
*  최종 모델 검증 : 숏폼 콘텐츠를 활용하여 지능평가 수행 __accuracy 0.33__
*  검증용 데이터 : 짧은대본의 ‘이별여행’, 숏박스의 ‘찐남매’, 빌런즈의 ‘개념없는신입 vs 젊은 꼰대’ (연구 활용 동의 완료)
