가상환경 생성 
```
conda create -n jupyterlab 
```

생성한 가상환경 활성화
```
conda activate jupyterlab
```

가상환경에 주피터 랩 설치
```
pip install jupyterlab
```

주피터 랩 실행
```
jupyter lab 
```

브라우저 자동으로 열리지 않게 설정
```
jupyter lab --no-browser
```

## Jupyter 가상환경 추가하기
1. 가상환경 생성 (이미 했으면 스킵)
2. 가상환경 활성화 
```
conda activate [$ENVIRONMENT_NAME]
```
3. 가상환경 내 ipykernel 설치
```
pip install ipykernel 
```
4.jupyter 가상환경 내 환경 등록
```
python -m ipykernel install --user --name [$ENVIRONMENT_NAME] --display-name [$KERNEL_NAME]
```
5. 활성화할 Kernel 선택
6. Kernel 삭제
```
jupyter kernelspec uninstall [$KERNEL_NAME]
