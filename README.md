# MedicalNer

- ���ĵ��Ӳ�������ʵ��ʶ��(pytorchʵ��)
### ���ݼ�����

- ��ѹ data_origin.zip, ���� transfer_data.py,�õ���ע�����ݼ�
- �����Լ������ȡtrain,test,dev�������ݼ�

### �޸�����config.yml
    embedding_size: 300
    hidden_size: 128
    model_path: models/
    batch_size: 30
    dropout: 0.5
    tags:
      - TREATMENT
      - BODY
      - SIGNS
      - CHECK
      - DISEASE
### ѵ��

- ȷ������ʱ��GPU,��Ȼ��Ҫ�޸Ĳ��ִ��� (��torch.cuda()������.cuda() ɾ��)
- ͨ�����ݼ��������ݵõ� train,test,dev �������ݼ�
- ����main.py

        1.python main.py
        2.���� train ���ɿ�ʼѵ��
        3.ѵ������
        
        epoch [70] |������������������������������������������������ | 29/30
            loss 141.02		time 11.984375
        --------------------------------------------------
        epoch [70] |��������������������������������������������������| 30/30
            loss 140.33		time 10.21875
        --------------------------------------------------
        epoch  70 avg_loss  231.88453776041666 total_time  693.546875
            TREATMENT	orgins:805.0	founds:803.0	rights:782.0
                recall:0.9714285714285714	precision:0.9738480697384807	f1:0.9726368159203981
            BODY	orgins:8278.0	founds:8262.0	rights:7915.0
                recall:0.9561488282193766	precision:0.958000484144275	f1:0.9570737605804112
            SIGNS	orgins:6366.0	founds:6356.0	rights:6309.0
                recall:0.9910461828463714	precision:0.9926054122089364	f1:0.9918251847193837
            CHECK	orgins:7718.0	founds:7757.0	rights:7633.0
                recall:0.9889867841409692	precision:0.9840144385716127	f1:0.9864943457189015
            DISEASE	orgins:474.0	founds:465.0	rights:436.0
                recall:0.919831223628692	precision:0.9376344086021505	f1:0.9286474973375931
            all_orgins:23641.0	all_founds:23643.0	all_rights:23075.0
            all_recall:0.9760585423628442	all_precision:0.975975975975976	all_f1:0.9760172574232299
        ----------------------------------------------------------------------------------------------------
        
### Ԥ��
- ����main.py

        1.python main.py
        2.���� predict ���ɿ�ʼԤ��
        3.�����ı�
        
### ����
- ��Ҫ���������ݼ�����Ϊ test
- ����main.py

        1.python main.py
        2.���� evaluate ���ɿ�ʼ����



