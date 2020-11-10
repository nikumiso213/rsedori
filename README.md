# README

## usersテーブル

| Column   | Type   | Options     |
| -------- | ------ | ----------- |
| nickname | string | null: false |
| email    | string | null: false |
| password | string | null: false |

### Association

- has_many : points
- has_many : profits

## pointsテーブル
| Column          | Type    | Options     |
| --------------- | ------- | ----------- |
| r_member_id     | integer | null: false |
| r_mobile_id     | integer | null: false |
| r_hikari_id     | integer | null: false |
| r_pgcard_id     | integer | null: false |
| r_bank_id       | integer | null: false |
| r_insurance_id  | integer | null: false |
| r_electrical_id | integer | null: false |
| r_securities_id | integer | null: false |
| r_travel_id     | integer | null: false |
| r_app_id        | integer | null: false |
| r_books_id      | integer | null: false |
| r_kobo_id       | integer | null: false |
| r_pasha_id      | integer | null: false |
| r_fashion_id    | integer | null: false |
| r_tv_id         | integer | null: false |
| r_beauty_id     | integer | null: false |

### Association

- belongs_to : user
- has_many   : profits

## profitsテーブル
| Column     | Type    | Options     |
| ---------- | ------- | ----------- |
| price      | string  | null: false |
| delivery   | string  | null: false |
| fee        | string  | null: false |
| p_shop     | string  | 
| p_campaign | string  | 
| p_marathon | string  |
| p_05day    | integer | 

### Association

- belongs_to : user
- belongs_to : point