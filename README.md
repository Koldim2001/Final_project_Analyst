# А/А/B тестирование

__Выполнил__: Колесников Дмитрий

![](https://cdn-icons-png.flaticon.com/128/8003/8003056.png)

# Условие проекта:

Вы работаете в крупном дейтинговом приложении (приложении для знакомств).

Помимо базовых функций, в приложении также имеется премиум-подписка, которая дает доступ к ряду важных дополнительных возможностей. Был проведен A/B тест, в рамках которого для новых пользователей из нескольких стран была изменена стоимость премиум-подписки* при покупке через две новые платежные системы. При этом стоимость пробного периода оставалась прежней.

## Проверьте :

1. Был ли эксперимент успешен в целом.
2. Проанализируйте, имеет ли нововведение смысл среди каких-либо конкретных групп пользователей.

💬 Деньги за подписку списываются ежемесячно до тех пор, пока пользователь её не отменит.

---
### Информация о данных:

**Всего есть три группы:** тестовая (test), контрольная 1 (control_1) и контрольная 2 (control_2). Для каждой из них:

<aside>
📄 users_*.csv – информация о пользователях:

</aside>

**uid** – идентификатор пользователя <br>
**age** – возраст <br>
**attraction_coeff** – коэффициент привлекательности (значение в диапазоне от 0 до 1000) - соотношение числа лайков к показам, умноженное на 1000 <br>
**coins** – число монеток (внутренняя валюта) <br>
**country** – страна  <br>
**visit_days** – в какие дни после регистрации пользователь посещал приложение (напр. в 1, затем в 7) <br>
***gender*** – пол <br>
**age_filter_start**  – фильтр поиска, мин. значение <br>
**age_filter_end**  – фильтр поиска, макс. значение <br>
**views_count** – число полученных оценок <br>
**was_premium** – был ли когда-либо премиум (либо пробный период премиум-статуса, либо купленный за деньги) <br>
**is_premium** –  является ли премиум <br>
**total_revenue** – нормированная выручка <br>

<aside>
📄 transactions_*.csv – информация о платежах пользователей:

</aside>

**uid** – идентификатор пользователя <br>
**country** – страна <br>
**joined_at** – дата и время регистрации <br>
**paid_at** – дата и время покупки <br>
**revenue** – нормированная выручка <br>
**payment_id** – идентификатор платежа <br>
**from_page** – откуда пользователь перешел на страницу оплаты <br>
**product_type** – тип продукта 
(*trial_premium* – пробная премиум-подписка, *premium_no_trial* – премиум-подписка без пробной, *coins* – подписка за внутреннюю валюту, *other_type* – другое) 

---
> Решение данного проекта представлено в формате документа [AAB_test.ipynb](https://github.com/Koldim2001/Final_project_Analyst/blob/main/AAB_test.ipynb)
>
