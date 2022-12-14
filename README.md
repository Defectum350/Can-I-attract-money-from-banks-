# Can-I-attract-money-from-banks-
### Целью данной работы является анализ датасета клиентов банка, с последующим выявлением определенных закономерностей
### А также вычленение необходимых фичей с дальнейшим машинным обучением для классификации клиентов на 3 фундаментальные группы
#### ID: Представляет уникальный идентификатор записи
#### Customer_ID: Представляет уникальную идентификацию человека
#### Month: Представляет месяц года
#### Name: Представляет имя человека
#### Age: Представляет возраст человека
#### SSN: Представляет номер социального страхования человека
#### Occupation: Представляет род занятий человека
#### Annual_Income: Представляет собой годовой доход человека
#### Monthly_Inhand_Salary: Представляет собой месячную базовую заработную плату человека.
#### Num_Bank_Accounts: Представляет собой количество банковских счетов, которыми владеет человек.
#### Num_Credit_Card: Представляет количество других кредитных карт, принадлежащих лицу
#### Interest_Rate: Представляет процентную ставку по кредитной карте
#### Num_of_Loan: Представляет количество кредитов, взятых в банке.
#### Type_of_Loan: Представляет виды кредита, взятого человеком
#### Delay_from_due_date: Представляет среднее количество дней задержки с даты платежа
#### Num_of_Delayed_Payment: Представляет среднее количество платежей, задержанных человеком
#### Changed_Credit_Limit: Представляет процентное изменение лимита кредитной карты
#### Num_Credit_Inquiries: Представляет количество запросов кредитной карты
#### Credit_Mix: Представляет классификацию сочетания кредитов
#### Outstanding_Debt: Представляет оставшуюся задолженность, подлежащую оплате (в долларах США)
#### Credit_Utilization_Ratio: Представляет коэффициент использования кредитной карты
#### Credit_History_Age: Представляет возраст кредитной истории человека
#### Payment_of_Min_Amount: Представляет, была ли уплачена только минимальная сумма лицом
#### Total_EMI_per_month: Представляет ежемесячные платежи EMI (в долларах США)
#### Amount_invested_monthly: Представляет ежемесячную сумму, инвестированную клиентом (в долларах США)
#### Payment_Behaviour: Представляет платежное поведение клиента (в долларах США)
#### Monthly_Balance: Представляет ежемесячную сумму баланса клиента (в долларах США)
#### Credit_Score: Представляет группу кредитного рейтинга (плохой, стандартный, хороший)
### После разведочного анализа данных, с последующим удалением не нужных на мой взгляд фичей, я приступаю к визуальному анализу данных
<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F.png?raw=true"/>

### При сравнении значений месяца нет большой разницы.
<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(1).png?raw=true"/>
<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(2).png?raw=true"/>
<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(3).png?raw=true"/>

### Порядок по количеству человек: 20, 30, 40, 10, 50.
### Порядок кредитного рейтинга: 50, 40, 30, 20, 10.
### Кредитный рейтинг большинства людей является стандартным.
### Нет большой разницы между количеством людей с хорошим кредитным рейтингом в 20, 30, 40 лет.

<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(4).png?raw=true"/>

### Между профессиями нет большой разницы.

<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(5).png?raw=true"/>

### По мере увеличения количества банковских счетов кредитный рейтинг снижается.
### Форма падающего графика ближе к форме лестницы, чем к прямой.

<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(6).png?raw=true"/>

### По мере увеличения количества кредитных карт кредитный рейтинг уменьшается.
### Когда количество кредитных карт составляет 2-3 или 7-8, кредитный рейтинг значительно падает.

<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(7).png?raw=true"/>

### Когда процентная ставка составляет 89 и 2021, кредитный рейтинг значительно снижается.
### По мере увеличения процентной ставки кредитный рейтинг уменьшается.

<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(8).png?raw=true"/>

<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(9).png?raw=true"/>

### По мере увеличения количества кредитов кредитный рейтинг снижается.
### Количество людей, которые брали кредиты, больше всего в номерах 2, 3 и 4. И вы можете видеть, что есть даже люди, которые получили номера 8 и 9.
### Видно, что кредитный рейтинг резко падает от количества взятых кредитов с 1 на 2, с 4 на 5. В частности, действительно значительное снижение можно увидеть с 4 на #### 5.

<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(10).png?raw=true"/>

<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(11).png?raw=true"/>

### Большинству людей еще предстоит заплатить от 8 до 20 видов денег.
### Чем выше количество просроченных платежей, тем ниже кредитный рейтинг, который почти прямой.

<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(12).png?raw=true"/>

<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(13).png?raw=true"/>

### Кредитный микс, оплата минимальной суммы, имеет прямое отношение к кредитному рейтингу.

<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(14).png?raw=true"/>
<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(15).png?raw=true"/>

### Максимальное количество людей в группе Low_spent_Medium_value_payments. Но их кредитные рейтинги самые низкие.
### Люди из группы High_spent_Large_value_payments имеют лучшие кредитные рейтинги.

<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(16).png?raw=true"/>

### Можно видеть, что ежемесячный баланс наибольшего числа людей по группе кредитного рейтинга тем выше, чем лучше кредитный рейтинг.

<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(17).png?raw=true"/>

### Люди с хорошим кредитным рейтингом имеют более высокое распределение месячной заработной платы, чем люди со средним или плохим кредитным рейтингом.

<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(18).png?raw=true"/>

### Люди с хорошим кредитным рейтингом имеют более высокое распределение годового дохода, чем люди со средним или плохим кредитом.
### Если вы посмотрите на график годового дохода, а не на график месячной заработной платы, вы сможете увидеть разницу между тремя группами более четко.

<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(19).png?raw=true"/>
<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(20).png?raw=true"/>
<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(21).png?raw=true"/>
<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(22).png?raw=true"/>

### Распределение категорий кредитного рейтинга следующее: Стандартный рейтинг занимает 53% распределения, плохой 29% и 18% хороший
### После визуального анализа данных я устранил дисбаланс классов при помощи SMOTE метода
### Выбрал XGBClassifier и обучил модель на всех тренировочных данных

<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(23).png?raw=true"/>

### Визуализировав confusion matrix, проглядывается то, что модель отлично справляется с классификацией всех 3 классов практически в равной мере
### Теперь необходимо сделать предикт на новых тестовых данных и в следствии визуального анализа выявить какие-либо аномалии в новых данных

<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(24).png?raw=true"/>
<img src="https://github.com/Defectum350/images/blob/main/%D0%BC%D0%BE%D0%B3%D1%83%20%D0%BB%D0%B8/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20(25).png?raw=true"/>

### Соотношение по возрастному диапозону также сильно не отличается от распределения в размеченном датасете












