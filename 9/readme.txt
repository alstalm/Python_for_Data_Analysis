�������� ������� �� ������ 9: "API �������� Google"

*********************************************************************

�������� �������:
=================

��������� ��� ������ ������ �� ����������� ���� �� 12-18 ������� 2018 ����. ���������� ����� ������� � ���� ������. � �������� ������ ��������� ������ ������������ ��������� ���� ��������. ��� ���������� �������� ������� report, ������� �� �������� start_index � max_results ���������� ��������� ������ ����� ������:

start_index = 1

max_results = 500

results = []

while True:

    print('������� �������� ��� start_index = {}'.format(start_index))

    data = report(start_index, max_results)

    

    if len(data) == 0:

        break

    

    results += data

    

    start_index += max_results