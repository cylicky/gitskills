git config --global user.name ''  �Լ����زֿ������
git config  --global user.email '' �Լ��������ַ

���ش���һ������ֿ�
makdir name  �����ļ�
git init �ѵ�ǰ�ļ��б��Git����ֿ�
git add .   ���ļ���ӵ�Git�ݴ�����
git commit -m '�汾˵��'  �ݴ����ύ�����ؿ�
������Ϣ
1 file changed��1���ļ����Ķ�����������ӵ�readme.txt�ļ�����
2 insertions����������������

git reset --hard  '�汾��'  �л��汾��
git  log/reflog  �鿴�汾��

git chenckout --file ���ظո��޸ĵ��ļ�
git status �鿴�ļ�״̬

git reset HEAD . �����ύ���ݴ������ļ�

git remote add origin ���Ͽ�·�� 
git branch -M main ������֧
git push -u origin main �ϴ������ϵķ�֧

�鿴��֧��git branch
������֧��git branch <name>
�л���֧��git checkout <name>����git switch <name>
����+�л���֧��git checkout -b <name>����git switch -c <name>
�ϲ�ĳ��֧����ǰ��֧��git merge <name>
ɾ����֧��git branch -d <name>