# MIT_Convlstm2d
# 진행했던 작업:MIT에서 제공하는 환자들의 데이터를 딥러닝진행으로 뇌전증 유무를 판별

# 사용한 데이터:MIT에서 제공하는 24명 환자의 데이터(EDF),환자 뇌파의 체널정보와 뇌전증 유무를 담은 텍스트 파일(txt)

# 데이터 전처리 방법: EDF 파일을 시각화(Visualization part.ipynb) 후 딥러닝을 할수 있도록 STFT 진행후(Data_preprocessing.ipynb),위치 정보를 추가해 H5 file로 저장(Make_hdf5_stft_preprocessing.ipynb)

# 사용한 딥러닝 기법:Convlstm2d

# Convlstm2d 사용한 이유:lstm을 이용할 경우 환자의 시간정보 이용만 가능하지만 데이터의 핵심인 환자의 뇌파 체널 데이터를 사용하지 못하기 때문에(convlstm_edf_second.ipynb)

# 뇌전증 판단기준: 각 초마다 딥러닝 전에 설정한 sec_frame번의 결과가 나오게 된다. 정상은 0 뇌전증 의심은 1 해당초의 점수 기준이 넘어가면 최종 뇌전증으로 확정한다. 
