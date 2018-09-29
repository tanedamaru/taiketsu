# README
## topicテーブル

|Column|Type|Options|
|------|----|-------|
|topic_id|integer|null: false, foreign_key: true|
|topic_title|string|null: false, foreign_key: false|


### Association
- has_many :comment

## commentテーブル

|Column|Type|Options|
|------|----|-------|
|comment_id|integer|null: false, foreign_key: true|
|comment_content|string|null: false, foreign_key: false|
|good_count|integer|null: false, foreign_key: false|
|bad_count|integer|null: false, foreign_key: false|
|which|integer|null: false, foreign_key: false|

### Association
- belongs_to :topic