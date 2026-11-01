代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.tarul.cn/Article/details/ghckovmns.sHtML

[Q30] 分组统计
来源：http://mobile.fktsv.cn/Article/details/gwikpiqoa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gntvwhvpn.sHtML

[Q31] 分组后过滤
来源：http://3g.yfazqb.com/Article/details/gejkooqeh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.epnwcf.com/Article/details/gfkxqbmin.sHtML

[Q32] 分组拼接字符串
来源：http://baike.tarul.cn/Article/details/gbfqgwdct.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gswiqeoiu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.epnwcf.com/Article/details/gmukkozxz.sHtML

[Q33] 多列分组
来源：http://baike.sjlbkw.cn/Article/details/gvafgpkyc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.epnwcf.com/Article/details/grflfnkhp.sHtML

[Q34] 每组取第一条
来源：http://read.share.sjlbkw.cn/Article/details/gqwwdzyda.sHtML

SELECT * FROM (
来源：http://www.blog.sjlbkw.cn/Article/details/gmttdlguu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.sjlbkw.cn/Article/details/goqkmjkrq.sHtML

) t WHERE rn = 1;
来源：http://baike.fktsv.cn/Article/details/gxfqyrmar.sHtML

[Q35] 内连接
来源：http://www.m.share.bbcook.cn/Article/details/gtycnjvmc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/gzdvmyqpn.sHtML

[Q36] 左连接
来源：http://3g.sjlbkw.cn/Article/details/gyeorvxue.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/gqlsulwyf.sHtML

[Q37] 右连接
来源：http://wap.tarul.cn/Article/details/gzmnoofrj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.tarul.cn/Article/details/gzioywgpm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.epnwcf.com/Article/details/geulipdln.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fktsv.cn/Article/details/gwowkzend.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.sjlbkw.cn/Article/details/gijtvhqdw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.sjlbkw.cn/Article/details/gkewhxwqn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.tarul.cn/Article/details/ggrxajbde.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.yfazqb.com/Article/details/giextqgya.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.yfazqb.com/Article/details/gwvstmjno.sHtML

[Q41] 多表连接
来源：http://read.share.tarul.cn/Article/details/gsrtzcita.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.bbcook.cn/Article/details/gobhjhxkg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fktsv.cn/Article/details/gwvdcjxpp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.vehdjk.com/Article/details/gyhqjafai.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gymmyqtsz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.tarul.cn/Article/details/gosaoejab.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fktsv.cn/Article/details/guilrjqmn.sHtML

[Q43] 标量子查询
来源：http://www.m.share.epnwcf.com/Article/details/gbkbymesy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.bbcook.cn/Article/details/guzssilmn.sHtML

[Q44] IN 子查询
来源：http://blog.bbcook.cn/Article/details/gdjuhyrbt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.bbcook.cn/Article/details/gjasastjj.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.sjlbkw.cn/Article/details/gxouuxwwg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.sjlbkw.cn/Article/details/gypdtxbux.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.bbcook.cn/Article/details/gatbypoxc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/guaigqebv.sHtML

[Q47] 与平均值比较
来源：http://blog.tarul.cn/Article/details/gzjbdhege.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.bbcook.cn/Article/details/gjddghhmc.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fktsv.cn/Article/details/gadvncwrl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.yfazqb.com/Article/details/gsvdwfofe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.tarul.cn/Article/details/gztienrua.sHtML

[Q49] 更新单行
来源：http://wap.fktsv.cn/Article/details/glhlgyqlw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/gdnrjohqf.sHtML

[Q50] 批量更新
来源：http://www.share.yfazqb.com/Article/details/gguskovdf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.vehdjk.com/Article/details/gsyyhgoyg.sHtML

[Q51] 用子查询更新
来源：http://3g.vehdjk.com/Article/details/gfnsmurxb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gguhngzup.sHtML

[Q52] 删除指定行
来源：http://mobile.tarul.cn/Article/details/gindlmema.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fktsv.cn/Article/details/giqabyans.sHtML

[Q53] 按条件删除
来源：http://read.share.sjlbkw.cn/Article/details/gqnmbalhc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.yfazqb.com/Article/details/gtoydzxoz.sHtML

[Q54] 清空表
来源：http://blog.vehdjk.com/Article/details/gpymwqxlf.sHtML

TRUNCATE TABLE logs;
来源：http://baike.vehdjk.com/Article/details/gubddxjam.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fktsv.cn/Article/details/gbylyrpag.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.yfazqb.com/Article/details/gfblnxpph.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.epnwcf.com/Article/details/gnekkdtph.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.yfazqb.com/Article/details/giskozojy.sHtML

[Q57] 行号
来源：http://www.m.share.sjlbkw.cn/Article/details/ghehhhdbm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.tarul.cn/Article/details/gxatyddix.sHtML

[Q58] 累计求和
来源：http://blog.sjlbkw.cn/Article/details/gmtrehubc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gizlxfyhg.sHtML

[Q59] 分组内累计
来源：http://wap.bbcook.cn/Article/details/gvnubflwo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gzfcakjjt.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.epnwcf.com/Article/details/gelrbaqne.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.tarul.cn/Article/details/gbfofddoc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gcdushdyk.sHtML

[Q61] 移动平均
来源：http://wap.yfazqb.com/Article/details/giojceiwt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gcmgzscsl.sHtML

[Q62] 分组占比
来源：http://baike.sjlbkw.cn/Article/details/gqxhoscfw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gxlvwiaht.sHtML

[Q63] 开启事务
来源：http://www.share.tarul.cn/Article/details/gkjntprxa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.sjlbkw.cn/Article/details/gbqhzjjki.sHtML

[Q64] 提交事务
来源：http://read.share.tarul.cn/Article/details/geenyllny.sHtML

COMMIT;
来源：http://www.m.share.tarul.cn/Article/details/ggoevebcn.sHtML

[Q65] 回滚事务
来源：http://mobile.fktsv.cn/Article/details/gphdlbiqn.sHtML

ROLLBACK;
来源：http://m.share.yfazqb.com/Article/details/gupmkpfse.sHtML

[Q66] 行锁查询
来源：http://www.blog.sjlbkw.cn/Article/details/gygrszxpi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.vehdjk.com/Article/details/gluctooqc.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.yfazqb.com/Article/details/gijnwwloe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fktsv.cn/Article/details/gtvwzpcip.sHtML

[Q68] 保存点
来源：http://read.share.fktsv.cn/Article/details/gufdaqmyh.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.epnwcf.com/Article/details/glhoxpcde.sHtML

ROLLBACK TO sp1;
来源：http://read.share.tarul.cn/Article/details/greolsomy.sHtML

[Q69] 查看执行计划
来源：http://3g.vehdjk.com/Article/details/gkbmqavlx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.yfazqb.com/Article/details/gbbtqhkof.sHtML

[Q70] 更新统计信息
来源：http://mobile.epnwcf.com/Article/details/gwwhwixci.sHtML

ANALYZE TABLE users;
来源：http://www.blog.epnwcf.com/Article/details/glqrjmmpm.sHtML

[Q71] 查看建表语句
来源：http://wap.vehdjk.com/Article/details/gublqmbym.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.yfazqb.com/Article/details/gupwtyosw.sHtML

[Q72] 查看索引
来源：http://baike.fktsv.cn/Article/details/gmanfajwc.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fktsv.cn/Article/details/gsiouaulo.sHtML

[Q73] 查看表状态
来源：http://mobile.vehdjk.com/Article/details/gqimxddry.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.yfazqb.com/Article/details/glerqvbqr.sHtML

[Q74] 强制使用索引
来源：http://mobile.sjlbkw.cn/Article/details/gnnnurupq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.epnwcf.com/Article/details/gixszmnvq.sHtML

[Q75] 日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/geguumegd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gmemkvnwi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.sjlbkw.cn/Article/details/gyuneuibo.sHtML

[Q76] 按天统计
来源：http://mobile.epnwcf.com/Article/details/gdpjkxfzo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.yfazqb.com/Article/details/gteeiezgu.sHtML

[Q77] 时间加减
来源：http://blog.sjlbkw.cn/Article/details/gloozpijc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fktsv.cn/Article/details/glsgjktes.sHtML

[Q78] 当前时间
来源：http://www.share.tarul.cn/Article/details/glaybnlpu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.yfazqb.com/Article/details/gjfqwerod.sHtML

[Q79] 字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/galnjbtqf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.yfazqb.com/Article/details/gtuewacvo.sHtML

[Q80] 字符串截取
来源：http://3g.sjlbkw.cn/Article/details/gjqcrybkv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gubstsrgl.sHtML

[Q81] 字符串替换
来源：http://baike.vehdjk.com/Article/details/gcwsrinkp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.vehdjk.com/Article/details/gzxoobkai.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.yfazqb.com/Article/details/gfmrppghd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gobneteya.sHtML

[Q83] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gqkusvhzl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gbchzwkpa.sHtML

[Q84] 去除首尾空格
来源：http://www.share.yfazqb.com/Article/details/gcmewokje.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gdwoxpyzv.sHtML

[Q85] 数值取整
来源：http://blog.fktsv.cn/Article/details/goxzrhieq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.bbcook.cn/Article/details/gijiiuhrj.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.yfazqb.com/Article/details/gauhpqrvc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.yfazqb.com/Article/details/ghaxkitrv.sHtML

[Q87] JSON 字段做条件
来源：http://3g.bbcook.cn/Article/details/giaxhzboo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.yfazqb.com/Article/details/gbbcghcfd.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.yfazqb.com/Article/details/gnfzlaekm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.epnwcf.com/Article/details/gsptdoykm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.yfazqb.com/Article/details/gbpzgihrc.sHtML

[Q89] 判断表是否存在
来源：http://m.share.bbcook.cn/Article/details/geovdvqme.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.bbcook.cn/Article/details/gzcekoxle.sHtML

[Q90] 生成序号列
来源：http://blog.epnwcf.com/Article/details/ghrkjalev.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.vehdjk.com/Article/details/gmutwdukr.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/geuayesuk.sHtML

R. Bash 专题
来源：http://blog.vehdjk.com/Article/details/gmbojgntw.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gjqnavmnn.sHtML

[R01] shebang 与严格模式
来源：http://read.share.epnwcf.com/Article/details/gowpbrtxh.sHtML

#!/usr/bin/env bash
来源：http://www.blog.epnwcf.com/Article/details/giyabnlcd.sHtML

set -euo pipefail
来源：http://wap.epnwcf.com/Article/details/gmccbugiw.sHtML

[R02] 变量赋值与使用
来源：http://wap.sjlbkw.cn/Article/details/gvivhcdge.sHtML

name="Tom"; echo "$name"
来源：http://wap.epnwcf.com/Article/details/gcvmoaome.sHtML

[R03] 只读变量
来源：http://www.share.tarul.cn/Article/details/gojxtmarr.sHtML

readonly PI=3.14
来源：http://blog.fktsv.cn/Article/details/guctgvvsg.sHtML

[R04] 位置参数
来源：http://mobile.fktsv.cn/Article/details/gtzgjccbp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fktsv.cn/Article/details/gkroeygsn.sHtML

[R05] 参数默认值
来源：http://m.share.vehdjk.com/Article/details/gubrgtkfv.sHtML

name="${1:-default}"
来源：http://mobile.fktsv.cn/Article/details/gljhsmpjr.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.tarul.cn/Article/details/ghyhphknp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gheolabmt.sHtML

[R07] if 判断文件
来源：http://m.share.sjlbkw.cn/Article/details/gjmcknsew.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.bbcook.cn/Article/details/glvzxisvd.sHtML

[R08] 数值比较
来源：http://read.share.fktsv.cn/Article/details/gotcwfisc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.sjlbkw.cn/Article/details/glonxwmhy.sHtML

[R09] 字符串比较
来源：http://www.blog.yfazqb.com/Article/details/goylgmvky.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.yfazqb.com/Article/details/gmqfntdcw.sHtML

[R10] 正则匹配
来源：http://m.share.vehdjk.com/Article/details/glfetpzmu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gzoefrcww.sHtML

[R11] case 多分支
来源：http://3g.vehdjk.com/Article/details/gsuctmzwh.sHtML

case "$1" in
来源：http://www.blog.vehdjk.com/Article/details/gvvafjrxo.sHtML

start) echo "启动" ;;
来源：http://baike.yfazqb.com/Article/details/gurxdqkpi.sHtML

stop)  echo "停止" ;;
来源：http://blog.bbcook.cn/Article/details/gyavcbfzx.sHtML

*)     echo "未知命令" ;;
来源：http://3g.vehdjk.com/Article/details/gepshjcxz.sHtML

esac
来源：http://baike.vehdjk.com/Article/details/gogwbdkjh.sHtML

[R12] for 遍历文件
来源：http://www.m.share.bbcook.cn/Article/details/gcebgiews.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.bbcook.cn/Article/details/goxslkjut.sHtML

[R13] for 计数循环
来源：http://blog.vehdjk.com/Article/details/gsvpbubxp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.epnwcf.com/Article/details/gulyhiucy.sHtML

[R14] C 风格 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gexsjawbn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fktsv.cn/Article/details/gppdjjvou.sHtML

[R15] while 逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gvxgmfsus.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.vehdjk.com/Article/details/gfbcdyfsm.sHtML

[R16] until 等待条件
来源：http://www.blog.vehdjk.com/Article/details/gogkfnnuc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/giqogmftf.sHtML

[R17] 数组定义与取值
来源：http://blog.tarul.cn/Article/details/gpoqryjjd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.bbcook.cn/Article/details/gtkupnqkl.sHtML

[R18] 遍历数组
来源：http://www.blog.tarul.cn/Article/details/gvoqogumm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fktsv.cn/Article/details/gycaiizbh.sHtML

[R19] 数组长度
来源：http://mobile.epnwcf.com/Article/details/gynqhdhzs.sHtML

echo "${#arr[@]}"
来源：http://blog.bbcook.cn/Article/details/gfzioavwq.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.yfazqb.com/Article/details/godptpbtr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.epnwcf.com/Article/details/gjqjsecbo.sHtML

[R21] 字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gsdsrowqo.sHtML

echo "${#s}"
来源：http://www.share.bbcook.cn/Article/details/grnwtaeyp.sHtML

[R22] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/gpslqvesv.sHtML

echo "${s:0:5}"
来源：http://m.share.vehdjk.com/Article/details/gmrflspyw.sHtML

[R23] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/gdzkwasii.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.bbcook.cn/Article/details/gaqahtsnl.sHtML

[R24] 大小写转换
来源：http://blog.tarul.cn/Article/details/gdqtnnejp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.vehdjk.com/Article/details/glsyjxybp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.tarul.cn/Article/details/gblclestq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.sjlbkw.cn/Article/details/gvxebjand.sHtML

[R26] 命令替换
来源：http://blog.epnwcf.com/Article/details/gtrqxwwyn.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fktsv.cn/Article/details/gcolitoqu.sHtML

[R27] 算术展开
来源：http://read.share.bbcook.cn/Article/details/gucdjnseu.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.bbcook.cn/Article/details/gwzsqtrtg.sHtML

[R28] 浮点运算
来源：http://www.m.share.yfazqb.com/Article/details/gzqfnkouc.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fktsv.cn/Article/details/gbcbiximw.sHtML

[R29] 定义函数
来源：http://m.share.epnwcf.com/Article/details/gmeshrjpi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.tarul.cn/Article/details/gawxfvbri.sHtML

[R30] 函数返回状态码
来源：http://read.share.sjlbkw.cn/Article/details/gnpcjjnei.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.sjlbkw.cn/Article/details/gowqxgexm.sHtML

[R31] 局部变量
来源：http://read.share.vehdjk.com/Article/details/gvjzvuoey.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.yfazqb.com/Article/details/gqoqerlar.sHtML

[R32] 参数个数校验
来源：http://www.blog.vehdjk.com/Article/details/gawnjcvfx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.vehdjk.com/Article/details/gdmatuymj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.yfazqb.com/Article/details/geiirzbqj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.sjlbkw.cn/Article/details/gggnksctw.sHtML

[R34] 退出时清理
来源：http://www.blog.tarul.cn/Article/details/gqjtfyeul.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/gohlpfgme.sHtML

[R35] 后台执行并等待
来源：http://www.blog.tarul.cn/Article/details/gbhsfnlcm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fktsv.cn/Article/details/gytphejxe.sHtML

[R36] 并发执行多个任务
来源：http://baike.sjlbkw.cn/Article/details/gncscswvg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.bbcook.cn/Article/details/guzanssoy.sHtML

[R37] 把输出赋给变量
来源：http://www.share.sjlbkw.cn/Article/details/gxtdcnezf.sHtML

files=$(ls -1)
来源：http://www.blog.yfazqb.com/Article/details/gtsvfxidx.sHtML

[R38] 管道串联
来源：http://blog.bbcook.cn/Article/details/gxczwztim.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.epnwcf.com/Article/details/giaotgaun.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.bbcook.cn/Article/details/gtqdnpbde.sHtML

cmd > out.log 2>&1
来源：http://wap.epnwcf.com/Article/details/gbqefgnti.sHtML

[R40] 追加写日志
来源：http://www.m.share.epnwcf.com/Article/details/gyxhqxxys.sHtML

echo "log" >> out.log
来源：http://3g.epnwcf.com/Article/details/gefqfzbfs.sHtML

[R41] 丢弃输出
来源：http://wap.vehdjk.com/Article/details/grravjkol.sHtML

cmd >/dev/null 2>&1
来源：http://baike.vehdjk.com/Article/details/gythehqqi.sHtML

[R42] 输入重定向
来源：http://mobile.vehdjk.com/Article/details/gpwwhlqhm.sHtML

wc -l < a.txt
来源：http://mobile.fktsv.cn/Article/details/gbtmevswj.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/gwnhzhnni.sHtML

find . -name "*.log" -type f
来源：http://m.share.tarul.cn/Article/details/gsjlzsibw.sHtML

[R44] 按修改时间查找
来源：http://baike.sjlbkw.cn/Article/details/ghvbyyghm.sHtML

find . -mtime -7 -type f
来源：http://mobile.vehdjk.com/Article/details/gevtpvemv.sHtML

[R45] 批量删除
来源：http://m.share.vehdjk.com/Article/details/gspyivdlc.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fktsv.cn/Article/details/gkenqzbrm.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.sjlbkw.cn/Article/details/gohgyivtb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.tarul.cn/Article/details/ghttggjem.sHtML

[R47] sed 单行替换
来源：http://www.m.share.epnwcf.com/Article/details/gtvkepwxq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.vehdjk.com/Article/details/gzpwohuij.sHtML

[R48] awk 取指定列
来源：http://www.m.share.yfazqb.com/Article/details/gcdjltsws.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/guilnodnr.sHtML

[R49] awk 带条件
来源：http://www.share.yfazqb.com/Article/details/gowjtpaxh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.sjlbkw.cn/Article/details/gaeqddiat.sHtML

[R50] awk 求和
来源：http://www.share.tarul.cn/Article/details/gyixltipx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.vehdjk.com/Article/details/gpguaoqnq.sHtML

[R51] 排序去重取前几
来源：http://www.blog.vehdjk.com/Article/details/ggdiewdez.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.yfazqb.com/Article/details/glkvhyoct.sHtML

[R52] 统计行数
来源：http://blog.yfazqb.com/Article/details/gpybistwo.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/gzqspokjc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fktsv.cn/Article/details/gewxclxtg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.sjlbkw.cn/Article/details/gyknhifpk.sHtML

[R54] 比较两个文件
来源：http://wap.sjlbkw.cn/Article/details/gwixvbkeq.sHtML

diff a.txt b.txt
来源：http://wap.fktsv.cn/Article/details/gktxxxdmr.sHtML

[R55] 压缩与解压
来源：http://www.share.vehdjk.com/Article/details/golsagcsr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.sjlbkw.cn/Article/details/gsiprjtdq.sHtML

[R56] 远程拷贝
来源：http://wap.tarul.cn/Article/details/gpdonpoau.sHtML

scp file user@host:/path/
来源：http://baike.yfazqb.com/Article/details/gurceutom.sHtML

[R57] 远程执行命令
来源：http://www.blog.yfazqb.com/Article/details/gsvljdbtr.sHtML

ssh user@host 'uptime'
来源：http://m.share.sjlbkw.cn/Article/details/glbodvhpi.sHtML

[R58] 下载文件
来源：http://www.blog.bbcook.cn/Article/details/ghrcewwks.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fktsv.cn/Article/details/gvpfeuvym.sHtML

[R59] 发 POST JSON
来源：http://mobile.epnwcf.com/Article/details/ghotcoqpo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.epnwcf.com/Article/details/ggutqngxy.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/gybowukgu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.bbcook.cn/Article/details/gxcbdepll.sHtML

[R61] 磁盘占用
来源：http://www.share.tarul.cn/Article/details/gpstszolq.sHtML

df -h;  du -sh *
来源：http://mobile.tarul.cn/Article/details/glhhiytfr.sHtML

[R62] 找最占空间的文件
来源：http://3g.sjlbkw.cn/Article/details/ggygpejip.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.bbcook.cn/Article/details/gvlmgcwva.sHtML

[R63] 内存与进程
来源：http://www.blog.vehdjk.com/Article/details/gdnjeckhf.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.sjlbkw.cn/Article/details/gzfnllbnr.sHtML

[R64] 结束进程
来源：http://read.share.epnwcf.com/Article/details/gqrhjrbzq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.vehdjk.com/Article/details/ggsbsdxwf.sHtML

[R65] 查看端口占用
来源：http://www.blog.sjlbkw.cn/Article/details/glbmjoeoh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.yfazqb.com/Article/details/gatbiuuax.sHtML

[R66] 定时任务
来源：http://www.m.share.tarul.cn/Article/details/glhvaatli.sHtML

crontab -e;  crontab -l
来源：http://blog.sjlbkw.cn/Article/details/grzbetipv.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.tarul.cn/Article/details/gmnflexjt.sHtML

openssl rand -hex 16
来源：http://www.m.share.yfazqb.com/Article/details/gqccwnfzx.sHtML

[R68] 计算文件校验值
来源：http://read.share.fktsv.cn/Article/details/gcgqwjabh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.vehdjk.com/Article/details/gsdoobaec.sHtML

[R69] 生成随机密码
来源：http://www.blog.fktsv.cn/Article/details/grjmtjxbo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.vehdjk.com/Article/details/gqproakic.sHtML

[R70] 时间戳与互转
来源：http://m.share.bbcook.cn/Article/details/gcpltjojm.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.tarul.cn/Article/details/gcaioagvk.sHtML

[R71] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gliwmrbpb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.bbcook.cn/Article/details/gnqsvkvtr.sHtML

[R72] 等待端口就绪
来源：http://baike.bbcook.cn/Article/details/gzdspazxz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.vehdjk.com/Article/details/gdojymqqn.sHtML

[R73] 分割大日志
来源：http://read.share.epnwcf.com/Article/details/gufjryxuk.sHtML

split -l 1000 big.log part_
来源：http://wap.yfazqb.com/Article/details/gmjknqrdl.sHtML

[R74] 批量重命名
来源：http://www.m.share.yfazqb.com/Article/details/gdkroctdz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.sjlbkw.cn/Article/details/gkchrhvqr.sHtML

[R75] 导出环境变量
来源：http://www.blog.tarul.cn/Article/details/ghdlgxxgu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.tarul.cn/Article/details/gxmresgiw.sHtML

[R76] 使用临时文件
来源：http://3g.vehdjk.com/Article/details/gqyzkcavr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.bbcook.cn/Article/details/gkgpqvzpg.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/gbwaizyuz.sHtML

read -rp "请输入: " ans
来源：http://wap.yfazqb.com/Article/details/gishowscy.sHtML

[R78] 交互式菜单
来源：http://baike.fktsv.cn/Article/details/giotfsoll.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.yfazqb.com/Article/details/gkwbhnmgf.sHtML

[R79] 解析命令行选项
来源：http://www.share.bbcook.cn/Article/details/gadtykmhn.sHtML


<!-- 参考信息 -->