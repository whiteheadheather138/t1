代发 wailian999

[Q33] 多列分组
来源：http://wap.sjlbkw.cn/Article/details/gewlefhhd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fktsv.cn/Article/details/gljnodvuw.sHtML

[Q34] 每组取第一条
来源：http://www.share.vehdjk.com/Article/details/gukngyzvj.sHtML

SELECT * FROM (
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbfcdvhk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.vehdjk.com/Article/details/gidhsntcu.sHtML

) t WHERE rn = 1;
来源：http://blog.sjlbkw.cn/Article/details/gawhcoygs.sHtML

[Q35] 内连接
来源：http://www.blog.tarul.cn/Article/details/glttwmewb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.yfazqb.com/Article/details/gheqgfkps.sHtML

[Q36] 左连接
来源：http://blog.fktsv.cn/Article/details/gtxcbymes.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/gtkxzurli.sHtML

[Q37] 右连接
来源：http://3g.fktsv.cn/Article/details/gexgcwcbi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.tarul.cn/Article/details/gzwcnubrn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.epnwcf.com/Article/details/gejojrpuk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.epnwcf.com/Article/details/gzagcmjhr.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.vehdjk.com/Article/details/gffxponbe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.yfazqb.com/Article/details/gfnecbdwr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.vehdjk.com/Article/details/gzbsbvwzf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.vehdjk.com/Article/details/ggnfzkfap.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.tarul.cn/Article/details/gfnrhyeza.sHtML

[Q41] 多表连接
来源：http://www.share.bbcook.cn/Article/details/gnobnldiw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.sjlbkw.cn/Article/details/guaqeaqzp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.vehdjk.com/Article/details/gqaldqrac.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fktsv.cn/Article/details/gvxmsbyyb.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.sjlbkw.cn/Article/details/gboskziyj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.epnwcf.com/Article/details/gmehlbijr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.yfazqb.com/Article/details/gztaxtcdm.sHtML

[Q43] 标量子查询
来源：http://www.share.sjlbkw.cn/Article/details/gwabljind.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.tarul.cn/Article/details/giommigiu.sHtML

[Q44] IN 子查询
来源：http://www.share.epnwcf.com/Article/details/ggqvwwpzh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.epnwcf.com/Article/details/gsdnwlvsu.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.sjlbkw.cn/Article/details/gkzyniwvf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gffnkmmnf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fktsv.cn/Article/details/gqofqborl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/gsmrimwvp.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.epnwcf.com/Article/details/gptjggobx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fktsv.cn/Article/details/gmtwukqww.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.vehdjk.com/Article/details/gjyapeamv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.vehdjk.com/Article/details/gdmzsuyyo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.vehdjk.com/Article/details/gsgnteqff.sHtML

[Q49] 更新单行
来源：http://wap.fktsv.cn/Article/details/glrjwblbv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.sjlbkw.cn/Article/details/ghfkjmndf.sHtML

[Q50] 批量更新
来源：http://wap.sjlbkw.cn/Article/details/gvbomjtum.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.vehdjk.com/Article/details/gonchbyry.sHtML

[Q51] 用子查询更新
来源：http://m.share.bbcook.cn/Article/details/gfewsivza.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.tarul.cn/Article/details/glfnxufli.sHtML

[Q52] 删除指定行
来源：http://blog.yfazqb.com/Article/details/gulokfwss.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gmjfnwwaq.sHtML

[Q53] 按条件删除
来源：http://baike.tarul.cn/Article/details/gmwjdwwsh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.epnwcf.com/Article/details/gdixzqqkw.sHtML

[Q54] 清空表
来源：http://www.share.epnwcf.com/Article/details/gtngeiehv.sHtML

TRUNCATE TABLE logs;
来源：http://wap.yfazqb.com/Article/details/gdakbflrq.sHtML

[Q55] 排名（并列占位）
来源：http://3g.bbcook.cn/Article/details/gntekdnnm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.sjlbkw.cn/Article/details/grhhmchni.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.bbcook.cn/Article/details/glsprzocs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.vehdjk.com/Article/details/gifamxtxy.sHtML

[Q57] 行号
来源：http://3g.bbcook.cn/Article/details/gpkcxzccg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gsfhwizfh.sHtML

[Q58] 累计求和
来源：http://baike.sjlbkw.cn/Article/details/gxxrgkwjj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gigqmzxaz.sHtML

[Q59] 分组内累计
来源：http://wap.tarul.cn/Article/details/gddulqqag.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gahkbbztb.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.sjlbkw.cn/Article/details/gqephefql.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.bbcook.cn/Article/details/gtfjahnsy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.vehdjk.com/Article/details/gcgwfxfqk.sHtML

[Q61] 移动平均
来源：http://3g.vehdjk.com/Article/details/gytdwqdyu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gpzkjdswn.sHtML

[Q62] 分组占比
来源：http://baike.fktsv.cn/Article/details/ghnqezmpl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/gazhjrrsu.sHtML

[Q63] 开启事务
来源：http://read.share.vehdjk.com/Article/details/gilgicqpb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.tarul.cn/Article/details/ggodglenv.sHtML

[Q64] 提交事务
来源：http://www.share.vehdjk.com/Article/details/gkaozzqjn.sHtML

COMMIT;
来源：http://blog.vehdjk.com/Article/details/gdrxslcry.sHtML

[Q65] 回滚事务
来源：http://www.blog.bbcook.cn/Article/details/gxwmlgalr.sHtML

ROLLBACK;
来源：http://www.m.share.tarul.cn/Article/details/gkxngyfno.sHtML

[Q66] 行锁查询
来源：http://mobile.epnwcf.com/Article/details/gdnnxclnr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.sjlbkw.cn/Article/details/ghpmdfrbc.sHtML

[Q67] 设置隔离级别
来源：http://mobile.epnwcf.com/Article/details/gsaxgeoxp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.tarul.cn/Article/details/gvohadzih.sHtML

[Q68] 保存点
来源：http://3g.bbcook.cn/Article/details/gycyunlgc.sHtML

SAVEPOINT sp1;
来源：http://blog.bbcook.cn/Article/details/goukfnwwn.sHtML

ROLLBACK TO sp1;
来源：http://wap.vehdjk.com/Article/details/gzjnyhblk.sHtML

[Q69] 查看执行计划
来源：http://mobile.epnwcf.com/Article/details/gmtkiwagq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.epnwcf.com/Article/details/gpzsvdrur.sHtML

[Q70] 更新统计信息
来源：http://baike.epnwcf.com/Article/details/gmoaijmtz.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.epnwcf.com/Article/details/gjyxhkstr.sHtML

[Q71] 查看建表语句
来源：http://3g.vehdjk.com/Article/details/gvrhgxwuj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fktsv.cn/Article/details/gkyampltw.sHtML

[Q72] 查看索引
来源：http://baike.yfazqb.com/Article/details/gbauioexl.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gvsttaqfi.sHtML

[Q73] 查看表状态
来源：http://www.m.share.bbcook.cn/Article/details/goiobhuhj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.yfazqb.com/Article/details/ghkkenmqq.sHtML

[Q74] 强制使用索引
来源：http://mobile.fktsv.cn/Article/details/gjzhzhfnn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.sjlbkw.cn/Article/details/gpokriivo.sHtML

[Q75] 日期格式化
来源：http://blog.epnwcf.com/Article/details/gzngipgnr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.vehdjk.com/Article/details/gtglkkpcv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.sjlbkw.cn/Article/details/grdtbjvnb.sHtML

[Q76] 按天统计
来源：http://read.share.fktsv.cn/Article/details/gavrrerns.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.bbcook.cn/Article/details/gvbxtvpoa.sHtML

[Q77] 时间加减
来源：http://m.share.epnwcf.com/Article/details/geeomffnr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.bbcook.cn/Article/details/gbhabnalz.sHtML

[Q78] 当前时间
来源：http://m.share.vehdjk.com/Article/details/groesjguk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.tarul.cn/Article/details/gudoqsovh.sHtML

[Q79] 字符串拼接
来源：http://baike.yfazqb.com/Article/details/gsfxgruhg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.epnwcf.com/Article/details/gcupmscyg.sHtML

[Q80] 字符串截取
来源：http://www.share.yfazqb.com/Article/details/gnrsvfjhw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gxgvrwbgf.sHtML

[Q81] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/grlviwake.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gdjxzvvcn.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.bbcook.cn/Article/details/gfkufjlie.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gpfhhczri.sHtML

[Q83] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gtuboyjql.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gkjiuorwn.sHtML

[Q84] 去除首尾空格
来源：http://wap.yfazqb.com/Article/details/ghyufaqne.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/galryfzfy.sHtML

[Q85] 数值取整
来源：http://www.m.share.tarul.cn/Article/details/gwxifbrmy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.yfazqb.com/Article/details/gzceadfwt.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fktsv.cn/Article/details/gbamssegr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fktsv.cn/Article/details/ggjlouwvb.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.yfazqb.com/Article/details/guaavirwk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.vehdjk.com/Article/details/gogkcwzqv.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.yfazqb.com/Article/details/gqsahzajb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fktsv.cn/Article/details/gsfjrghdc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.tarul.cn/Article/details/gsiifbzcu.sHtML

[Q89] 判断表是否存在
来源：http://m.share.epnwcf.com/Article/details/gfvxnkqwi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.epnwcf.com/Article/details/grhorzesy.sHtML

[Q90] 生成序号列
来源：http://3g.fktsv.cn/Article/details/gkfizsrdk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.bbcook.cn/Article/details/glmnglels.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkbpvoveo.sHtML

R. Bash 专题
来源：http://www.m.share.yfazqb.com/Article/details/gloebnxoe.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/grivscvjt.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.epnwcf.com/Article/details/gopmkjndo.sHtML

#!/usr/bin/env bash
来源：http://read.share.bbcook.cn/Article/details/ghyhfjqto.sHtML

set -euo pipefail
来源：http://mobile.bbcook.cn/Article/details/gmpjuyhkw.sHtML

[R02] 变量赋值与使用
来源：http://baike.vehdjk.com/Article/details/gqejsnjiy.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.epnwcf.com/Article/details/gdrwuqtnw.sHtML

[R03] 只读变量
来源：http://mobile.epnwcf.com/Article/details/gxndcnilt.sHtML

readonly PI=3.14
来源：http://www.blog.sjlbkw.cn/Article/details/gvujavrhs.sHtML

[R04] 位置参数
来源：http://blog.bbcook.cn/Article/details/gvjdujncq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.sjlbkw.cn/Article/details/greaygaii.sHtML

[R05] 参数默认值
来源：http://baike.bbcook.cn/Article/details/gnybpvzrj.sHtML

name="${1:-default}"
来源：http://blog.fktsv.cn/Article/details/ghkrssfhl.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gzwnofszm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/gqlwzqlmi.sHtML

[R07] if 判断文件
来源：http://blog.epnwcf.com/Article/details/gmpacnumm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.epnwcf.com/Article/details/grluvokpj.sHtML

[R08] 数值比较
来源：http://m.share.vehdjk.com/Article/details/gnoadncdd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fktsv.cn/Article/details/gwstrbqwh.sHtML

[R09] 字符串比较
来源：http://baike.fktsv.cn/Article/details/gwurzoofa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.vehdjk.com/Article/details/gsexyfkxz.sHtML

[R10] 正则匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gglzvrlhw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.tarul.cn/Article/details/gamwrcioh.sHtML

[R11] case 多分支
来源：http://blog.bbcook.cn/Article/details/gvfkkqtgu.sHtML

case "$1" in
来源：http://m.share.epnwcf.com/Article/details/gayfspite.sHtML

start) echo "启动" ;;
来源：http://wap.yfazqb.com/Article/details/glsdbipyh.sHtML

stop)  echo "停止" ;;
来源：http://www.share.epnwcf.com/Article/details/gosoldrvi.sHtML

*)     echo "未知命令" ;;
来源：http://wap.bbcook.cn/Article/details/gygkhlgtu.sHtML

esac
来源：http://3g.epnwcf.com/Article/details/gsslrrucm.sHtML

[R12] for 遍历文件
来源：http://baike.vehdjk.com/Article/details/gdokhpzbk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.vehdjk.com/Article/details/gmergfkov.sHtML

[R13] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/gwgqsgdrc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/gwuwjiwsz.sHtML

[R14] C 风格 for
来源：http://mobile.tarul.cn/Article/details/grtjpgclh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/goiwlwjyj.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gsjqvlozh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.yfazqb.com/Article/details/gtdmlzqmb.sHtML

[R16] until 等待条件
来源：http://www.share.epnwcf.com/Article/details/gmwcvbvmk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.bbcook.cn/Article/details/gdgnfhgip.sHtML

[R17] 数组定义与取值
来源：http://www.blog.tarul.cn/Article/details/gvxehghst.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.yfazqb.com/Article/details/gnfbuhzbn.sHtML

[R18] 遍历数组
来源：http://www.share.tarul.cn/Article/details/ghrvgoyjs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.tarul.cn/Article/details/gnbvvjseh.sHtML

[R19] 数组长度
来源：http://read.share.yfazqb.com/Article/details/gbxekyfkr.sHtML

echo "${#arr[@]}"
来源：http://blog.yfazqb.com/Article/details/gtslmtqtn.sHtML

[R20] 关联数组（字典）
来源：http://m.share.vehdjk.com/Article/details/gqpdplvbh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.bbcook.cn/Article/details/gzngelxkh.sHtML

[R21] 字符串长度
来源：http://www.share.vehdjk.com/Article/details/genhpddem.sHtML

echo "${#s}"
来源：http://www.share.epnwcf.com/Article/details/gccyekgqn.sHtML

[R22] 截取子串
来源：http://mobile.vehdjk.com/Article/details/gpnqswgpq.sHtML

echo "${s:0:5}"
来源：http://read.share.vehdjk.com/Article/details/gcixecwho.sHtML

[R23] 字符串替换
来源：http://www.share.sjlbkw.cn/Article/details/gvsppmtlj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.vehdjk.com/Article/details/gfqexffxd.sHtML

[R24] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gpxdcjrye.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.sjlbkw.cn/Article/details/gioimcqks.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.tarul.cn/Article/details/gljrxrtvm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.sjlbkw.cn/Article/details/gwrmnaqva.sHtML

[R26] 命令替换
来源：http://www.blog.bbcook.cn/Article/details/gqaovrvcy.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.yfazqb.com/Article/details/gohwmzstn.sHtML

[R27] 算术展开
来源：http://m.share.vehdjk.com/Article/details/gzdqbvkas.sHtML

echo $((1 + 2 * 3))
来源：http://baike.epnwcf.com/Article/details/gfqzsizjs.sHtML

[R28] 浮点运算
来源：http://www.m.share.fktsv.cn/Article/details/ghrkmjmsg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.bbcook.cn/Article/details/gntpffgxo.sHtML

[R29] 定义函数
来源：http://wap.sjlbkw.cn/Article/details/ghnstdyon.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/gboaezhmb.sHtML

[R30] 函数返回状态码
来源：http://baike.bbcook.cn/Article/details/gmtesbjqy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.sjlbkw.cn/Article/details/gopszuodm.sHtML

[R31] 局部变量
来源：http://read.share.yfazqb.com/Article/details/gphbmshlq.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.bbcook.cn/Article/details/gpwdtkhzy.sHtML

[R32] 参数个数校验
来源：http://3g.fktsv.cn/Article/details/gahctiwtn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/gouaccxpa.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.tarul.cn/Article/details/ghvmnitkj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.vehdjk.com/Article/details/gqrjgqcuy.sHtML

[R34] 退出时清理
来源：http://baike.tarul.cn/Article/details/gnoejbfua.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/gnnixgski.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.yfazqb.com/Article/details/gvrwixddq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.bbcook.cn/Article/details/gnzwdoafv.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fktsv.cn/Article/details/gntnvuwqx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fktsv.cn/Article/details/gxmoogfjk.sHtML

[R37] 把输出赋给变量
来源：http://www.share.epnwcf.com/Article/details/gfgpbkuux.sHtML

files=$(ls -1)
来源：http://baike.sjlbkw.cn/Article/details/gcepdplzb.sHtML

[R38] 管道串联
来源：http://baike.tarul.cn/Article/details/gpubkqpiq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.tarul.cn/Article/details/grrtdikyg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fktsv.cn/Article/details/gekvhczex.sHtML

cmd > out.log 2>&1
来源：http://m.share.bbcook.cn/Article/details/ghrfrnmah.sHtML

[R40] 追加写日志
来源：http://blog.fktsv.cn/Article/details/gavwjqtgo.sHtML

echo "log" >> out.log
来源：http://baike.tarul.cn/Article/details/gdrpphjno.sHtML

[R41] 丢弃输出
来源：http://www.m.share.tarul.cn/Article/details/ggkqmlokr.sHtML

cmd >/dev/null 2>&1
来源：http://blog.sjlbkw.cn/Article/details/geijyzibh.sHtML

[R42] 输入重定向
来源：http://read.share.yfazqb.com/Article/details/ghugtcqna.sHtML

wc -l < a.txt
来源：http://wap.tarul.cn/Article/details/gbbrlpjdr.sHtML

[R43] 按名字查找文件
来源：http://mobile.epnwcf.com/Article/details/gedvbgkzn.sHtML

find . -name "*.log" -type f
来源：http://www.blog.yfazqb.com/Article/details/gqxkzjwve.sHtML

[R44] 按修改时间查找
来源：http://m.share.epnwcf.com/Article/details/gxhgejhme.sHtML

find . -mtime -7 -type f
来源：http://mobile.sjlbkw.cn/Article/details/gqkjpximr.sHtML

[R45] 批量删除
来源：http://www.m.share.tarul.cn/Article/details/gccuqryqg.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.epnwcf.com/Article/details/gzlszhvyh.sHtML

[R46] 递归替换文件内容
来源：http://3g.sjlbkw.cn/Article/details/gmskqhfix.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.bbcook.cn/Article/details/gkbhaozje.sHtML

[R47] sed 单行替换
来源：http://baike.fktsv.cn/Article/details/guzasthhf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gifeqjkyo.sHtML

[R48] awk 取指定列
来源：http://m.share.vehdjk.com/Article/details/gvxeqddjq.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gokpfwusu.sHtML

[R49] awk 带条件
来源：http://blog.bbcook.cn/Article/details/gympsrmwo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.yfazqb.com/Article/details/greucdntz.sHtML

[R50] awk 求和
来源：http://3g.fktsv.cn/Article/details/ghyetvdyt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gbbwrswtc.sHtML

[R51] 排序去重取前几
来源：http://www.blog.epnwcf.com/Article/details/gpynvvduk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.yfazqb.com/Article/details/gcsayxkaz.sHtML

[R52] 统计行数
来源：http://read.share.sjlbkw.cn/Article/details/gxnighoud.sHtML

wc -l a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gfcmfzovv.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.tarul.cn/Article/details/gqmvdfckd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.vehdjk.com/Article/details/gvjhmpjrg.sHtML

[R54] 比较两个文件
来源：http://mobile.bbcook.cn/Article/details/gnpxjyhuh.sHtML

diff a.txt b.txt
来源：http://baike.sjlbkw.cn/Article/details/gyaijqqdk.sHtML

[R55] 压缩与解压
来源：http://www.m.share.yfazqb.com/Article/details/gpisorrjx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.vehdjk.com/Article/details/glmiwkcgk.sHtML

[R56] 远程拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gidiqiogj.sHtML

scp file user@host:/path/
来源：http://mobile.sjlbkw.cn/Article/details/ghkqejvbk.sHtML

[R57] 远程执行命令
来源：http://www.blog.sjlbkw.cn/Article/details/grkuzegmc.sHtML

ssh user@host 'uptime'
来源：http://m.share.vehdjk.com/Article/details/gloqwrwjk.sHtML

[R58] 下载文件
来源：http://baike.bbcook.cn/Article/details/gufbbrrqk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.yfazqb.com/Article/details/gmwitoqvv.sHtML

[R59] 发 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/goqnhbzhz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fktsv.cn/Article/details/gqhtmlgrx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/gycargdxp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fktsv.cn/Article/details/gmlsgehir.sHtML

[R61] 磁盘占用
来源：http://blog.epnwcf.com/Article/details/gjiafmjoz.sHtML

df -h;  du -sh *
来源：http://www.blog.fktsv.cn/Article/details/giadkgrxb.sHtML

[R62] 找最占空间的文件
来源：http://3g.vehdjk.com/Article/details/gmvmgbxmz.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.epnwcf.com/Article/details/gsizisink.sHtML

[R63] 内存与进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnvelmbz.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.bbcook.cn/Article/details/gwrxmduhs.sHtML

[R64] 结束进程
来源：http://mobile.vehdjk.com/Article/details/gbxilljmf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.vehdjk.com/Article/details/giwtdsfmd.sHtML

[R65] 查看端口占用
来源：http://wap.sjlbkw.cn/Article/details/gfjzszjyx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.epnwcf.com/Article/details/gpckokdmn.sHtML

[R66] 定时任务
来源：http://mobile.tarul.cn/Article/details/gystvbbgf.sHtML

crontab -e;  crontab -l
来源：http://wap.epnwcf.com/Article/details/gcnfhcnys.sHtML

[R67] 生成随机十六进制串
来源：http://baike.yfazqb.com/Article/details/gfzhjyscv.sHtML

openssl rand -hex 16
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsubywet.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fktsv.cn/Article/details/gwradtivw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.yfazqb.com/Article/details/gzpvupewi.sHtML

[R69] 生成随机密码
来源：http://3g.yfazqb.com/Article/details/grsfxyuxi.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.yfazqb.com/Article/details/gzpjnxlgl.sHtML

[R70] 时间戳与互转
来源：http://blog.epnwcf.com/Article/details/gkbabomyq.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.sjlbkw.cn/Article/details/gnqkwgxnc.sHtML

[R71] 日期格式化
来源：http://blog.vehdjk.com/Article/details/gjrhnmozg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.yfazqb.com/Article/details/gdcaeskyk.sHtML

[R72] 等待端口就绪
来源：http://read.share.vehdjk.com/Article/details/gbjwebyaw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/goapdintq.sHtML

[R73] 分割大日志
来源：http://3g.epnwcf.com/Article/details/ghhpwqkwx.sHtML

split -l 1000 big.log part_
来源：http://m.share.tarul.cn/Article/details/gxxyhrefk.sHtML

[R74] 批量重命名
来源：http://blog.tarul.cn/Article/details/gemdnxbhk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.vehdjk.com/Article/details/gmbytciug.sHtML

[R75] 导出环境变量
来源：http://m.share.yfazqb.com/Article/details/gnjdxvxef.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.bbcook.cn/Article/details/ghibibdgp.sHtML

[R76] 使用临时文件
来源：http://baike.yfazqb.com/Article/details/gyejuvkqo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gxmwbisqz.sHtML

[R77] 读取用户输入
来源：http://read.share.sjlbkw.cn/Article/details/gjhktfysk.sHtML

read -rp "请输入: " ans
来源：http://read.share.bbcook.cn/Article/details/grfeirouy.sHtML

[R78] 交互式菜单
来源：http://www.blog.bbcook.cn/Article/details/guuylfuni.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.vehdjk.com/Article/details/gatpuihdx.sHtML

[R79] 解析命令行选项
来源：http://baike.epnwcf.com/Article/details/gcilzszbp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.bbcook.cn/Article/details/goptrajvm.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.sjlbkw.cn/Article/details/gvlnniamo.sHtML

time ./run.sh
来源：http://read.share.fktsv.cn/Article/details/gnvokpxav.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqmrlmxyc.sHtML

S. C / C++ 专题
来源：http://www.share.sjlbkw.cn/Article/details/gmhgfipjj.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/geuyslhdk.sHtML

[S01] C：Hello World
来源：http://mobile.vehdjk.com/Article/details/givxxgcek.sHtML

#include <stdio.h>
来源：http://blog.fktsv.cn/Article/details/gkiiehxak.sHtML


<!-- 参考信息 -->