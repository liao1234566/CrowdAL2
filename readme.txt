д��ƪreadme��Ŀ����ϣ�����ܹ��������֡����������ڰ��ģ�����ѧϰģ�͡�

Ŀ¼��
1 ����֪ʶ��
2 ���ݼ�˵��
3 ����˵��
4 ��ع��߰�˵��
5 ѧϰ����
6 ��������

1 ����֪ʶ��

	�ڰ�����
	����ѧϰ
	�ı�����
		���������ӣ��������ı�����ʽ
		http://www.jianshu.com/p/4cfcf1610a73 ��Python���ı���з���֮��м��Է�����
		http://blog.csdn.net/liugallup/article/details/51164962 ��ʹ��word2vec������΢��������з����ͷ��ࣩ
	����ѧϰ�㷨
		������������˽�һЩ����ѧϰ�㷨ԭ����Բο���ͳ��ѧϰ������� ��

2 ���ݼ�˵��
	
	1��������4000��΢��������ۼ��������ࣩ��������ȷ��ǩ��0,1�����ڰ��ռ��ı�ǩ����9���������ѡ�����Ķ�����ǩ�����ѡ5���Ķ�����ǩ��ԭʼ�ı����ݡ�
	     ������Դ��COAE2014
	     �ڰ���ǩ��Դ�������ڰ�
	     weibo/weibo_data_lablels_4000.txt 
	2��΢�����������ݼ���
	     ��Դ�������ڰ� 
	     weibo/weibo_feedback.xls
	     weibo/weibo_feedback_1.xls
	3��twitter���ݼ�������δ����
	     twitter/��б�ע_Twitter1000_9.xlsx
	4��ͣ�ôʡ������ķִ���Ҫ�õ�
	     stopword_chinese.txt
	5��ģ������Է���
	     CEF/ex0.txt

3 ����˵��
	
	data_preprocess.py 
		�ı�Ԥ�������ı�����Ԥ������TFIDFת��Ϊ��������
		input��
			ԭ�ı����ݼ� weibo_data_lablels_4000.txt 
			ͣ�ôʼ���stopword_chinese.txt��
		output�������� X

	weibo_baseline.py 
		�����������������ѧϰģ�͡�
		input��
			ԭ�ı����ݼ� weibo_data_lablels_4000.txt
		output����������ָ��

	weibo_al_margin.py
		���ڱ�Ե����������ѧϰģ�͡�
		input��ͬ�ϣ�output��ͬ��

	CEF_AL_weibo.py
		�����ڰ������Է���������ѧϰģ��
		input�� 
			weibo_data_labels_4000.txt �C ԭʼ����
			jieba_data.txt �C �ִ�����
  		        ex0.txt �C �˹���ѡ�Ľ����Է�����Ϣ
		output��
			mydata_disrupt.txt �C ������ԭʼ����
			selected_data.txt �C ��ѡ������ԭʼ��
			selected_data_jieba.txt �C ��ѡ�������ִʺ�
			��������ָ��

	plot_weibo_al_margin.py
		΢���ı����ӻ���������ӳ�䵽��άƽ�棬�������ѡ����������û������ɶ��������Ȥ�Ļ����Բο����룬����matplotlib����Ҳ�ܶࡣ

4 ��ع��߰�˵��
	
	numpy��scipy ���ھ�������
	pandas �������ݴ�ȡ
	jieba ���ķִ�
	sklearn ����ѧϰ�㷨
	matplotlib ���ݿ��ӻ�
	pickle �־û�ģ�͹���
	libact ����һ������ѧϰ�㷨���߰�

5 ѧϰ����

	�˽�����ѧϰ�㷨�������̣�
	�˽⴦���ı���������Ļ������̣�
	�˽�֧��������SVM��
	Ȼ���ٿ���data_preprocess.py��weibo_baseline.py ��weibo_al_margin.py
	����ٿ�������������ķ���CEF_AL_weibo.py��

6 �������� 
	
	1�����������ݼ����ɰ����ڰ��ռ����ݣ���һ��
	2�����ݼ�twitter��һ��ʵ��

PS��
������������ӭ�Ὠ�顣



														by cbw